<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Kyalo Fresh - Obulimi Bwaffe</title>

<script src="https://cdn.tailwindcss.com"></script>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">

<style>
body{
  font-family:Inter, sans-serif;
  overflow-x:hidden;
  background:#f8faf8;
}

html{
  scroll-behavior:smooth;
}

.hero-bg{
  background:
  linear-gradient(to top, rgba(0,0,0,.75), rgba(0,0,0,.35)),
  url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1600&auto=format&fit=crop');
  background-size:cover;
  background-position:center;
}

.card{
  transition:0.25s ease;
}

.card:hover{
  transform:translateY(-6px);
}

.safe-container{
  max-width:1200px;
  margin:auto;
  padding-left:16px;
  padding-right:16px;
}

/* MOBILE SAFETY FIX */
img{
  max-width:100%;
  height:auto;
  display:block;
}

button,a,input,select{
  font-size:16px;
}

</style>
</head>

<body class="text-gray-800 pt-20">

<!-- NAV -->
<header class="fixed top-0 left-0 w-full bg-white shadow z-50">

<div class="safe-container flex items-center justify-between h-16">

<!-- LOGO -->
<div class="flex items-center gap-3">

<div class="w-10 h-10 bg-green-600 rounded-full flex items-center justify-center text-white font-bold">
🌾
</div>

<div>
<h1 class="font-extrabold text-green-700 text-lg">Kyalo Fresh</h1>
<p class="text-xs text-gray-500">Obulimi bwaffe</p>
</div>

</div>

<!-- MENU -->
<nav class="hidden md:flex gap-6 font-semibold text-sm">
<a href="#market">Market</a>
<a href="#sell">Sell</a>
<a href="#ads">Ads</a>
</nav>

<a href="https://wa.me/256700000000"
class="bg-green-600 text-white px-4 py-2 rounded-full text-sm font-bold">
WhatsApp
</a>

</div>

</header>

<!-- HERO -->
<section class="hero-bg min-h-[90vh] flex items-center">

<div class="safe-container grid grid-cols-1 lg:grid-cols-2 gap-10">

<div class="text-center lg:text-left">

<h1 class="text-white font-black leading-tight text-4xl sm:text-5xl lg:text-6xl">
Sell Your Harvest Faster
</h1>

<p class="text-gray-200 mt-4 text-base sm:text-lg">
Kyalo Fresh connects farmers in Central Uganda directly to buyers.
</p>

<div class="flex flex-col sm:flex-row gap-4 mt-6">

<a href="#sell"
class="bg-green-600 text-white px-6 py-4 rounded-xl font-bold text-center">
Sell Produce
</a>

<a href="#market"
class="bg-white text-black px-6 py-4 rounded-xl font-bold text-center">
Browse Market
</a>

</div>

</div>

</div>

</section>

<!-- MARKET -->
<section id="market" class="py-16">

<div class="safe-container">

<h2 class="text-3xl font-bold mb-6">Marketplace</h2>

<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">

<!-- CARD -->
<div class="bg-white rounded-2xl shadow overflow-hidden card">

<img src="https://images.unsplash.com/photo-1603048297172-c92544798d5a?q=80&w=600&auto=format&fit=crop"
class="h-48 w-full object-cover"/>

<div class="p-4">

<h3 class="font-bold text-lg">Matooke</h3>
<p class="text-gray-500 text-sm">Kayunga</p>

<div class="flex justify-between mt-3 items-center">
<span class="text-green-700 font-bold">UGX 2,500</span>
<span class="text-xs bg-green-100 px-2 py-1 rounded-full">Fresh</span>
</div>

</div>

</div>

</div>

</div>

</section>

<!-- SELL -->
<section id="sell" class="py-16 bg-green-50">

<div class="safe-container">

<h2 class="text-3xl font-bold mb-6">Farmer Upload</h2>

<div class="grid grid-cols-1 lg:grid-cols-2 gap-8">

<!-- FORM -->
<form id="form" class="bg-white p-6 rounded-2xl shadow space-y-4">

<input id="name" placeholder="Product Name"
class="w-full border p-3 rounded-xl"/>

<input id="qty" placeholder="Quantity"
class="w-full border p-3 rounded-xl"/>

<input id="price" placeholder="Price"
class="w-full border p-3 rounded-xl"/>

<select id="loc" class="w-full border p-3 rounded-xl">
<option>Location</option>
<option>Kayunga</option>
<option>Mukono</option>
<option>Lugazi</option>
</select>

<button class="w-full bg-green-600 text-white p-3 rounded-xl font-bold">
Post Produce
</button>

</form>

<!-- LIVE LISTINGS -->
<div id="listings" class="space-y-4"></div>

</div>

</div>

</section>

<!-- ADS -->
<section id="ads" class="py-16">

<div class="safe-container">

<h2 class="text-3xl font-bold mb-6">Business Ads</h2>

<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">

<div class="bg-white p-6 rounded-2xl shadow">
Starter Package
</div>

<div class="bg-green-100 p-6 rounded-2xl shadow">
Pro Package
</div>

<div class="bg-white p-6 rounded-2xl shadow">
Enterprise
</div>

</div>

</div>

</section>

<!-- FOOTER -->
<footer class="bg-black text-white py-10">

<div class="safe-container text-center text-sm text-gray-300">
Kyalo Fresh © 2026 • Obulimi bwaffe
</div>

</footer>

<!-- WHATSAPP -->
<a href="https://wa.me/256700000000"
class="fixed bottom-5 right-5 bg-green-500 text-white w-14 h-14 rounded-full flex items-center justify-center text-2xl shadow-xl">
💬
</a>

<!-- SCRIPT -->
<script>

const form = document.getElementById("form");
const listings = document.getElementById("listings");

form.addEventListener("submit", function(e){
e.preventDefault();

const name = document.getElementById("name").value;
const qty = document.getElementById("qty").value;
const price = document.getElementById("price").value;
const loc = document.getElementById("loc").value;

const card = document.createElement("div");
card.className = "bg-white p-4 rounded-2xl shadow";

card.innerHTML = `
<b>${name}</b><br/>
${qty} • ${loc}<br/>
<span class="text-green-700 font-bold">${price}</span>
`;

listings.prepend(card);

form.reset();

});

</script>

</body>
</html>
