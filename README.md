<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Kyalo Fresh - Agri Startup</title>

<script src="https://cdn.tailwindcss.com"></script>

<style>
body{font-family:Inter,sans-serif;background:#f6f7f3;overflow-x:hidden;}
.card{transition:0.25s ease;}
.card:hover{transform:translateY(-5px);}
</style>
</head>

<body class="pt-20">

<!-- NAV -->
<div class="fixed top-0 w-full bg-white shadow z-50">
<div class="max-w-6xl mx-auto flex justify-between items-center p-4">
<h1 class="font-bold text-green-700">🌾 Kyalo Fresh</h1>
<a class="bg-green-600 text-white px-4 py-2 rounded-xl" href="#sell">Sell</a>
</div>
</div>

<!-- HERO -->
<section class="bg-green-800 text-white p-10 text-center">
<h1 class="text-3xl font-bold">Uganda Farm Marketplace</h1>
<p class="opacity-80">Sell & Buy Fresh Produce Directly</p>
</section>

<!-- LOGIN -->
<section class="max-w-md mx-auto p-4 mt-6 bg-white rounded-xl shadow">

<h2 class="font-bold mb-3">👨‍🌾 Farmer Login</h2>

<input id="email" placeholder="Email" class="w-full border p-3 rounded-xl mb-2">
<input id="password" type="password" placeholder="Password" class="w-full border p-3 rounded-xl mb-2">

<button onclick="login()" class="w-full bg-green-600 text-white p-3 rounded-xl mb-2">Login</button>
<button onclick="register()" class="w-full bg-black text-white p-3 rounded-xl">Register</button>

</section>

<!-- UPLOAD -->
<section id="sell" class="max-w-2xl mx-auto p-4 mt-6 bg-white rounded-xl shadow">

<h2 class="font-bold mb-3">🌾 Upload Produce</h2>

<input id="name" placeholder="Product" class="w-full border p-3 rounded-xl mb-2">
<input id="qty" placeholder="Quantity" class="w-full border p-3 rounded-xl mb-2">
<input id="price" placeholder="Price" class="w-full border p-3 rounded-xl mb-2">
<input id="loc" placeholder="Location" class="w-full border p-3 rounded-xl mb-2">
<input id="image" type="file" class="w-full border p-3 rounded-xl mb-2">

<button onclick="upload()" class="w-full bg-green-700 text-white p-3 rounded-xl">
Post Produce
</button>

</section>

<!-- CATALOGUE -->
<section class="max-w-6xl mx-auto p-4 mt-10">

<h2 class="font-bold text-xl mb-4">🛒 Live Catalogue</h2>

<div id="listings" class="grid grid-cols-2 md:grid-cols-4 gap-4"></div>

</section>

<!-- FIREBASE -->
<script type="module">

import { initializeApp } from "https://www.gstatic.com/firebasejs/10.7.1/firebase-app.js";
import { getAuth, createUserWithEmailAndPassword, signInWithEmailAndPassword, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/10.7.1/firebase-auth.js";
import { getFirestore, collection, addDoc, onSnapshot } from "https://www.gstatic.com/firebasejs/10.7.1/firebase-firestore.js";
import { getStorage, ref, uploadBytes, getDownloadURL } from "https://www.gstatic.com/firebasejs/10.7.1/firebase-storage.js";

/* 🔴 REPLACE WITH YOUR FIREBASE CONFIG */
const firebaseConfig = {
  apiKey: "YOUR_KEY",
  authDomain: "YOUR_PROJECT.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT.appspot.com",
  appId: "YOUR_APP"
};

const app = initializeApp(firebaseConfig);
const auth = getAuth(app);
const db = getFirestore(app);
const storage = getStorage(app);

let user = null;

/* LOGIN */
window.login = async ()=>{
const email = email.value;
const pass = password.value;
await signInWithEmailAndPassword(auth,email,pass);
alert("Logged in");
}

/* REGISTER */
window.register = async ()=>{
const email = email.value;
const pass = password.value;
await createUserWithEmailAndPassword(auth,email,pass);
alert("Account created");
}

/* AUTH STATE */
onAuthStateChanged(auth,(u)=>{
user = u;
});

/* UPLOAD */
window.upload = async ()=>{

if(!user){
alert("Login first");
return;
}

const file = image.files[0];

const storageRef = ref(storage,"products/"+Date.now());
await uploadBytes(storageRef,file);
const url = await getDownloadURL(storageRef);

await addDoc(collection(db,"products"),{
name:name.value,
qty:qty.value,
price:price.value,
location:loc.value,
image:url,
user:user.email
});

alert("Uploaded");

}

/* LIVE CATALOGUE */
const listings = document.getElementById("listings");

onSnapshot(collection(db,"products"),(snap)=>{

listings.innerHTML="";

snap.forEach(doc=>{
const d = doc.data();

listings.innerHTML += `
<div class="bg-white rounded-xl shadow overflow-hidden card">

<img src="${d.image}" class="h-28 w-full object-cover"/>

<div class="p-2">

<h3 class="font-bold">${d.name}</h3>
<p class="text-xs text-gray-500">${d.location}</p>

<div class="flex justify-between">
<span class="text-green-700 font-bold">${d.price}</span>
<span class="text-xs">${d.qty}</span>
</div>

<a href="https://wa.me/256700000000"
class="block mt-2 bg-green-600 text-white text-center p-2 rounded-xl text-sm">
Order
</a>

</div>

</div>
`;

});

});

</script>

</body>
</html>
