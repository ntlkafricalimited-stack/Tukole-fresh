
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Kyalo Fresh - Agri Catalogue</title>

<script src="https://cdn.tailwindcss.com"></script>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800;900&display=swap" rel="stylesheet">

<style>
body{
  font-family:Inter,sans-serif;
  background:#f6f7f3;
  overflow-x:hidden;
}

.hero{
  background:linear-gradient(135deg,#1b5e20,#2e7d32,#33691e);
}

.card{
  transition:0.25s ease;
}

.card:hover{
  transform:translateY(-5px);
}

.grid-catalogue{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(180px,1fr));
  gap:14px;
}

.badge{
  font-size:11px;
  padding:3px 8px;
  border-radius:999px;
}

</style>
</head>

<body>

<!-- TOP BAR -->
<div class="bg-green-900 text-white text-center text-xs py-2">
🌾 Kyalo Fresh Super Catalogue • Obulimi bwaffe • Buy Direct From Farmers
</div>

<!-- HERO -->
<section class="hero text-white px-5 py-10">

<div class="max-w-6xl mx-auto">

<h1 class="text-4xl md:text-6xl font-black leading-tight">
Uganda Farm<br>
<span class="text-yellow-300">Fresh Catalogue</span>
</h1>

<p class="mt-3 text-green-100">
Kayunga • Mukono • Lugazi • Kangulumira • Kalagi • Ndese
</p>

<div class="flex gap-3 mt-5">

<a href="#catalogue"
class="bg-yellow-400 text-black font-bold px-5 py-3 rounded-xl">
Browse Catalogue
</a>

<a href="#sell"
class="bg-white text-green-900 font-bold px-5 py-3 rounded-xl">
Sell Produce
</a>

</div>

</div>

</section>

<!-- CATEGORY BAR -->
<section class="px-4 py-5">

<div class="max-w-6xl mx-auto flex gap-2 overflow-x-auto">

<div class="bg-white px-4 py-2 rounded-full shadow text-sm">🌾 All</div>
<div class="bg-green-100 px-4 py-2 rounded-full text-sm">🍌 Matooke</div>
<div class="bg-white px-4 py-2 rounded-full shadow text-sm">🥕 Vegetables</div>
<div class="bg-white px-4 py-2 rounded-full shadow text-sm">🍊 Fruits</div>
<div class="bg-white px-4 py-2 rounded-full shadow text-sm">🌽 Grains</div>
<div class="bg-white px-4 py-2 rounded-full shadow text-sm">🥚 Eggs</div>

</div>

</section>

<!-- CATALOGUE -->
<section id="catalogue" class="px-4 py-6">

<div class="max-w-6xl mx-auto">

<h2 class="text-2xl font-bold mb-4">Super Catalogue</h2>

<div class="grid-catalogue">

<!-- ITEM 1 -->
<div class="bg-white rounded-2xl shadow overflow-hidden card">

<img src="https://images.unsplash.com/photo-1603048297172-c92544798d5a?q=80&w=600"
class="h-32 w-full object-cover">

<div class="p-3">

<h3 class="font-bold">Matooke</h3>
<p class="text-xs text-gray-500">Kayunga</p>

<div class="flex justify-between mt-2">
<span class="text-green-700 font-bold">UGX 2,500</span>
<span class="badge bg-green-100 text-green-700">Fresh</span>
</div>

<button class="mt-2 w-full bg-green-600 text-white py-2 rounded-xl text-sm">
Order
</button>

</div>

</div>

<!-- ITEM 2 -->
<div class="bg-white rounded-2xl shadow overflow-hidden card">

<img src="https://images.unsplash.com/photo-1615485500704-8e990f9900f0?q=80&w=600"
class="h-32 w-full object-cover">

<div class="p-3">

<h3 class="font-bold">Cassava</h3>
<p class="text-xs text-gray-500">Mukono</p>

<div class="flex justify-between mt-2">
<span class="text-green-700 font-bold">UGX 1,800</span>
<span class="badge bg-green-100 text-green-700">Fresh</span>
</div>

<button class="mt-2 w-full bg-green-600 text-white py-2 rounded-xl text-sm">
Order
</button>

</div>

</div>

<!-- ITEM 3 -->
<div class="bg-white rounded-2xl shadow overflow-hidden card">

<img src="https://images.unsplash.com/photo-1506806732259-39c2d0268443?q=80&w=600"
class="h-32 w-full object-cover">

<div class="p-3">

<h3 class="font-bold">Bananas</h3>
<p class="text-xs text-gray-500">Lugazi</p>

<div class="flex justify-between mt-2">
<span class="text-green-700 font-bold">UGX 3,000</span>
<span class="badge bg-green-100 text-green-700">Fresh</span>
</div>

<button class="mt-2 w-full bg-green-600 text-white py-2 rounded-xl text-sm">
Order
</button>

</div>

</div>

</div>

</div>

</section>

<!-- SELL -->
<section id="sell" class="px-4 py-10 bg-white">

<div class="max-w-6xl mx-auto">

<h2 class="text-2xl font-bold mb-4">Sell Your Produce</h2>

<form id="form" class="space-y-3">

<input id="name" placeholder="Product Name"
class="w-full border p-3 rounded-xl">

<input id="qty" placeholder="Quantity"
class="w-full border p-3 rounded-xl">

<input id="price" placeholder="Price"
class="w-full border p-3 rounded-xl">

<select id="loc" class="w-full border p-3 rounded-xl">
<option>Location</option>
<option>Kayunga</option>
<option>Mukono</option>
<option>Lugazi</option>
</select>

<button class="w-full bg-green-700 text-white p-3 rounded-xl font-bold">
Post To Catalogue
</button>

</form>

</div>

</section>

<!-- LIVE LISTINGS -->
<section class="px-4 py-10">

<div class="max-w-6xl mx-auto">

<h2 class="text-2xl font-bold mb-4">Live Farmer Listings</h2>

<div id="listings" class="grid-catalogue"></div>

</div>

</section>

<!-- FOOTER -->
<footer class="bg-green-950 text-white text-center py-8">

Kyalo Fresh Super Catalogue © 2026

</footer>

<!-- WHATSAPP -->
<a href="https://wa.me/256700000000"
class="fixed bottom-5 right-5 bg-green-500 w-14 h-14 rounded-full flex items-center justify-center text-2xl text-white shadow-xl">
💬
</a>

<!-- SCRIPT -->
<script>

const form = document.getElementById("form");
const listings = document.getElementById("listings");

form.addEventListener("submit",(e)=>{
e.preventDefault();

const name = document.getElementById("name").value;
const qty = document.getElementById("qty").value;
const price = document.getElementById("price").value;
const loc = document.getElementById("loc").value;

const div = document.createElement("div");
div.className="bg-white p-3 rounded-2xl shadow card";

div.innerHTML=`
<h3 class="font-bold">${name}</h3>
<p class="text-xs text-gray-500">${loc}</p>
<p class="text-green-700 font-bold">${price}</p>
<span class="text-xs">${qty}</span>
`;

listings.prepend(div);

form.reset();

});

</script>

</body>
</html>
