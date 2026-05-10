<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Kyalo Fresh - Obulimi Bwaffe</title>

<script src="https://cdn.tailwindcss.com"></script>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:'Inter',sans-serif;
overflow-x:hidden;
background:#f7faf7;
}

.hero-bg{
background:
linear-gradient(to top, rgba(0,0,0,.75), rgba(0,0,0,.35)),
url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1600&auto=format&fit=crop');
background-size:cover;
background-position:center;
}

.glass{
backdrop-filter:blur(14px);
background:rgba(255,255,255,.12);
border:1px solid rgba(255,255,255,.15);
}

.card{
transition:.3s ease;
}

.card:hover{
transform:translateY(-8px);
}

.market-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:1.5rem;
}

input,select{
outline:none;
}

</style>
</head>

<body class="text-gray-800">

<!-- TOP BAR -->
<div class="bg-green-900 text-white text-center text-sm py-2 px-4">
🌾 Kyalo Fresh • Fresh okuva mu byalo bya Uganda
</div>

<!-- NAVBAR -->
<header class="fixed top-0 left-0 w-full z-50 bg-white/95 backdrop-blur-md shadow-sm">

<div class="max-w-7xl mx-auto px-4 sm:px-6">

<div class="flex items-center justify-between h-20">

<!-- LOGO -->
<div class="flex items-center gap-3">

<div class="w-12 h-12 rounded-full bg-gradient-to-br from-green-600 to-orange-500 flex items-center justify-center text-white text-xl font-extrabold shadow-lg">
🌾
</div>

<div>
<h1 class="font-black text-2xl text-green-800">
Kyalo Fresh
</h1>

<p class="text-xs text-gray-500">
Obulimi bwaffe • Fresh Market
</p>
</div>

</div>

<!-- MENU -->
<nav class="hidden lg:flex items-center gap-8 font-semibold">

<a href="#market" class="hover:text-green-700 transition">
Market
</a>

<a href="#sell" class="hover:text-green-700 transition">
Sell Produce
</a>

<a href="#ads" class="hover:text-green-700 transition">
Business Ads
</a>

<a href="#locations" class="hover:text-green-700 transition">
Locations
</a>

</nav>

<!-- BTN -->
<a href="https://wa.me/256700000000"
class="bg-green-600 hover:bg-green-700 text-white px-5 py-3 rounded-full font-bold shadow-lg transition">

WhatsApp

</a>

</div>

</div>

</header>

<!-- HERO -->
<section class="hero-bg min-h-screen flex items-center pt-24">

<div class="max-w-7xl mx-auto px-6 w-full">

<div class="grid lg:grid-cols-2 gap-14 items-center">

<!-- LEFT -->
<div>

<div class="glass inline-flex items-center gap-2 text-white px-5 py-3 rounded-full mb-7">
🚜 Uganda Rural Marketplace
</div>

<h1 class="text-5xl md:text-7xl font-black text-white leading-tight">

Sell Your
<span class="text-green-400">
Harvest
</span>
Faster.

</h1>

<h2 class="text-2xl md:text-3xl text-orange-300 font-bold mt-5">
Gulisa Ebirime Byo Mangu.
</h2>

<p class="text-lg text-gray-200 leading-relaxed mt-8 max-w-2xl">

Kyalo Fresh helps farmers okuva e Kayunga,
Mukono, Lugazi, Kangulumira, Kalagi ne
Central Uganda okutunda produce directly
eri buyers.

</p>

<div class="flex flex-col sm:flex-row gap-5 mt-10">

<a href="#sell"
class="bg-green-600 hover:bg-green-700 text-white px-8 py-5 rounded-2xl text-lg font-bold shadow-2xl text-center">

🌾 Teeka Ebirime

</a>

<a href="#market"
class="bg-white hover:bg-gray-100 text-gray-900 px-8 py-5 rounded-2xl text-lg font-bold shadow-2xl text-center">

🛒 Browse Market

</a>

</div>

<!-- STATS -->
<div class="grid grid-cols-3 gap-4 mt-12">

<div class="glass p-5 rounded-2xl text-center">
<h3 class="text-3xl font-black text-white">
2,500+
</h3>

<p class="text-sm text-gray-200">
Farmers
</p>
</div>

<div class="glass p-5 rounded-2xl text-center">
<h3 class="text-3xl font-black text-white">
24/7
</h3>

<p class="text-sm text-gray-200">
Market
</p>
</div>

<div class="glass p-5 rounded-2xl text-center">
<h3 class="text-3xl font-black text-white">
8+
</h3>

<p class="text-sm text-gray-200">
Districts
</p>
</div>

</div>

</div>

<!-- RIGHT -->
<div>

<div class="bg-white rounded-[2rem] shadow-2xl p-7">

<div class="flex items-center justify-between mb-8">

<div>
<h3 class="text-2xl font-black text-green-800">
Fresh Listings
</h3>

<p class="text-gray-500">
Live okuva mu kyalo
</p>
</div>

<div class="bg-green-100 text-green-700 px-4 py-2 rounded-full text-sm font-bold">
LIVE
</div>

</div>

<div class="space-y-5">

<!-- CARD -->
<div class="flex items-center gap-4 bg-green-50 p-4 rounded-2xl card">

<img src="https://images.unsplash.com/photo-1603048297172-c92544798d5a?q=80&w=600&auto=format&fit=crop"
class="w-24 h-24 rounded-2xl object-cover">

<div class="flex-1">

<h4 class="font-black text-lg">
Fresh Matooke
</h4>

<p class="text-gray-500">
Kayunga • 500 bunches
</p>

</div>

<div class="text-right">

<h3 class="font-black text-green-700 text-2xl">
UGX 2,500
</h3>

<p class="text-sm text-gray-500">
per bunch
</p>

</div>

</div>

<!-- CARD -->
<div class="flex items-center gap-4 bg-orange-50 p-4 rounded-2xl card">

<img src="https://images.unsplash.com/photo-1542838132-92c53300491e?q=80&w=600&auto=format&fit=crop"
class="w-24 h-24 rounded-2xl object-cover">

<div class="flex-1">

<h4 class="font-black text-lg">
Vegetables
</h4>

<p class="text-gray-500">
Mukono • 300kg
</p>

</div>

<div class="text-right">

<h3 class="font-black text-orange-600 text-2xl">
UGX 3,000
</h3>

<p class="text-sm text-gray-500">
per kg
</p>

</div>

</div>

</div>

</div>

</div>

</div>

</div>

</section>

<!-- SELL SECTION -->
<section id="sell" class="py-24 bg-gradient-to-b from-green-50 to-white">

<div class="max-w-7xl mx-auto px-6">

<div class="text-center mb-14">

<h2 class="text-5xl font-black text-green-800">
Farmer Upload Portal
</h2>

<p class="text-gray-600 mt-5 text-lg">
Farmers can upload produce directly from phone or laptop.
</p>

</div>

<div class="grid lg:grid-cols-2 gap-10">

<!-- FORM -->
<div class="bg-white rounded-[2rem] shadow-2xl p-8 border border-green-100">

<form id="produceForm" class="space-y-5">

<input id="productName"
type="text"
placeholder="🌾 Product Name"
required
class="w-full border border-gray-200 rounded-2xl px-5 py-4">

<input id="quantity"
type="text"
placeholder="⚖ Quantity"
required
class="w-full border border-gray-200 rounded-2xl px-5 py-4">

<input id="price"
type="text"
placeholder="💰 Price"
required
class="w-full border border-gray-200 rounded-2xl px-5 py-4">

<select id="location"
required
class="w-full border border-gray-200 rounded-2xl px-5 py-4">

<option value="">📍 Select Location</option>
<option>Kayunga</option>
<option>Mukono</option>
<option>Lugazi</option>
<option>Kangulumira</option>
<option>Kalagi</option>

</select>

<input id="phone"
type="text"
placeholder="📞 Phone Number"
required
class="w-full border border-gray-200 rounded-2xl px-5 py-4">

<input id="image"
type="file"
accept="image/*"
required
class="w-full border border-dashed border-green-300 rounded-2xl p-4 bg-green-50">

<button
type="submit"
class="w-full bg-green-600 hover:bg-green-700 text-white py-5 rounded-2xl text-lg font-bold shadow-xl">

🚀 Upload Produce

</button>

</form>

</div>

<!-- LIVE LISTINGS -->
<div>

<div class="flex items-center justify-between mb-8">

<div>

<h3 class="text-3xl font-black text-green-800">
Live Farmer Listings
</h3>

<p class="text-gray-500">
Fresh uploads appear instantly
</p>

</div>

</div>

<div id="farmerListings" class="space-y-6"></div>

</div>

</div>

</div>

</section>

<!-- MARKET -->
<section id="market" class="py-24 bg-white">

<div class="max-w-7xl mx-auto px-6">

<div class="text-center mb-14">

<h2 class="text-5xl font-black text-green-800">
Buyer Marketplace
</h2>

<p class="text-gray-600 mt-5 text-lg">
Fresh produce direct okuva eri abalimi.
</p>

</div>

<!-- SEARCH -->
<div class="bg-green-50 rounded-3xl p-6 mb-14">

<div class="grid md:grid-cols-3 gap-5">

<input
type="text"
placeholder="🔍 Search produce..."
class="border border-gray-200 rounded-2xl px-5 py-4">

<select
class="border border-gray-200 rounded-2xl px-5 py-4">

<option>📍 All Locations</option>
<option>Kayunga</option>
<option>Mukono</option>

</select>

<button
class="bg-green-600 hover:bg-green-700 text-white rounded-2xl font-bold text-lg">

Search Market

</button>

</div>

</div>

<!-- PRODUCTS -->
<div class="market-grid">

<!-- CARD -->
<div class="bg-white rounded-3xl shadow-lg overflow-hidden card">

<img src="https://images.unsplash.com/photo-1603048297172-c92544798d5a?q=80&w=600&auto=format&fit=crop"
class="h-56 w-full object-cover">

<div class="p-6">

<h3 class="font-black text-2xl">
Matooke
</h3>

<p class="text-gray-500 mt-2">
📍 Kayunga
</p>

<div class="flex justify-between items-center mt-5">

<h3 class="text-3xl font-black text-green-700">
UGX 2,500
</h3>

<span class="bg-green-100 text-green-700 px-3 py-1 rounded-full text-sm font-bold">
Fresh
</span>

</div>

<button
class="w-full mt-6 bg-green-600 hover:bg-green-700 text-white py-4 rounded-2xl font-bold">

WhatsApp Order

</button>

</div>

</div>

</div>

</div>

</section>

<!-- ADS -->
<section id="ads" class="py-24 bg-green-900 text-white">

<div class="max-w-7xl mx-auto px-6 text-center">

<h2 class="text-5xl font-black">
Advertise Your Business
</h2>

<p class="text-green-100 mt-5 text-lg">
Agro-vets, transporters, shops, millers and suppliers.
</p>

<div class="grid md:grid-cols-3 gap-8 mt-14">

<div class="bg-white/10 p-8 rounded-3xl">

<h3 class="text-3xl font-black">
Starter
</h3>

<p class="text-5xl font-black mt-5">
50K
</p>

</div>

<div class="bg-orange-500 p-8 rounded-3xl shadow-2xl scale-105">

<h3 class="text-3xl font-black">
Pro
</h3>

<p class="text-5xl font-black mt-5">
150K
</p>

</div>

<div class="bg-white/10 p-8 rounded-3xl">

<h3 class="text-3xl font-black">
Enterprise
</h3>

<p class="text-5xl font-black mt-5">
Custom
</p>

</div>

</div>

</div>

</section>

<!-- FOOTER -->
<footer class="bg-black text-white py-16">

<div class="max-w-7xl mx-auto px-6 grid md:grid-cols-4 gap-10">

<div>

<h3 class="text-3xl font-black mb-5">
Kyalo Fresh
</h3>

<p class="text-gray-400">
Fresh okuva mu byalo byaffe.
</p>

</div>

<div>

<h4 class="font-bold text-xl mb-5">
Marketplace
</h4>

<ul class="space-y-3 text-gray-400">
<li>Buy Produce</li>
<li>Sell Produce</li>
<li>Farmer Accounts</li>
</ul>

</div>

<div>

<h4 class="font-bold text-xl mb-5">
Locations
</h4>

<ul class="space-y-3 text-gray-400">
<li>Kayunga</li>
<li>Mukono</li>
<li>Lugazi</li>
</ul>

</div>

<div>

<h4 class="font-bold text-xl mb-5">
Contact
</h4>

<ul class="space-y-3 text-gray-400">
<li>📞 +256 700 000000</li>
<li>📍 Central Uganda</li>
</ul>

</div>

</div>

</footer>

<!-- FLOATING BUTTON -->
<a href="https://wa.me/256700000000"
class="fixed bottom-6 right-6 bg-green-500 hover:bg-green-600 text-white w-16 h-16 rounded-full flex items-center justify-center text-3xl shadow-2xl z-50">

💬

</a>

<!-- SCRIPT -->
<script>

const form = document.getElementById("produceForm");
const listings = document.getElementById("farmerListings");

form.addEventListener("submit", function(e){

e.preventDefault();

const productName = document.getElementById("productName").value;
const quantity = document.getElementById("quantity").value;
const price = document.getElementById("price").value;
const location = document.getElementById("location").value;
const phone = document.getElementById("phone").value;
const imageInput = document.getElementById("image");

let imageURL = "https://images.unsplash.com/photo-1542838132-92c53300491e?q=80&w=600&auto=format&fit=crop";

if(imageInput.files[0]){
imageURL = URL.createObjectURL(imageInput.files[0]);
}

const card = document.createElement("div");

card.className =
"bg-white rounded-3xl shadow-lg overflow-hidden border border-green-100";

card.innerHTML = `

<div class="flex flex-col sm:flex-row">

<img
src="${imageURL}"
class="w-full sm:w-52 h-52 object-cover">

<div class="p-6 flex-1">

<div class="flex flex-col md:flex-row md:justify-between gap-5">

<div>

<h4 class="text-3xl font-black">
${productName}
</h4>

<p class="text-gray-500 mt-2">
📍 ${location}
</p>

</div>

<div>

<h3 class="text-3xl font-black text-green-700">
${price}
</h3>

<p class="text-sm text-gray-500">
market price
</p>

</div>

</div>

<div class="mt-5">

<span class="bg-green-100 text-green-700 px-4 py-2 rounded-full text-sm font-bold">
🌾 ${quantity}
</span>

</div>

<a href="https://wa.me/${phone.replace(/\+/g,'')}"
class="inline-flex items-center gap-2 mt-6 bg-green-600 hover:bg-green-700 text-white px-6 py-4 rounded-2xl font-bold">

💬 Contact Farmer

</a>

</div>

</div>

`;

listings.prepend(card);

form.reset();

window.scrollTo({
top:listings.offsetTop - 100,
behavior:"smooth"
});

});

</script>

</body>
</html>
