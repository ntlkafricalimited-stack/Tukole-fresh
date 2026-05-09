<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Kyalo Fresh - Marketplace</title>

  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

  <style>
    body { font-family: Inter, sans-serif; }

    .hero-bg{
      background:
      linear-gradient(to right, rgba(0,0,0,0.78), rgba(0,0,0,0.45)),
      url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1600&auto=format&fit=crop');
      background-size: cover;
      background-position: center;
    }

    .card { transition: 0.25s ease; }
    .card:hover { transform: translateY(-6px); }
  </style>
</head>

<body class="bg-gray-50 text-gray-800">

<!-- NAV -->
<header class="fixed top-0 left-0 w-full z-50 bg-white/95 backdrop-blur shadow">
  <div class="max-w-7xl mx-auto px-4 py-3 flex justify-between items-center">

    <div class="flex items-center gap-3">
      <div class="w-10 h-10 bg-green-600 rounded-full flex items-center justify-center text-white font-bold">K</div>
      <div>
        <h1 class="font-extrabold text-green-700">Kyalo Fresh</h1>
        <p class="text-xs text-gray-500">Obulimi bwaffe • Fresh Market</p>
      </div>
    </div>

    <nav class="hidden md:flex gap-6 text-sm font-medium">
      <a href="#market">Market</a>
      <a href="#sell">Sell</a>
      <a href="#ads">Ads</a>
      <a href="#locations">Locations</a>
    </nav>

    <button onclick="toggleDark()" class="px-3 py-1 bg-gray-100 rounded-full text-sm">🌙</button>

  </div>
</header>

<!-- HERO -->
<section class="hero-bg pt-28 min-h-screen flex items-center">
  <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-2 gap-10">

    <div class="text-white">
      <h1 class="text-4xl md:text-6xl font-extrabold leading-tight">
        Sell Your Harvest Faster.<br>
        <span class="text-green-400">Gulisa Ebirime Byo Mangu.</span>
      </h1>

      <p class="mt-6 text-gray-200">
        Kyalo Fresh connects farmers from Ndese, Kayunga, Mukono, Kangulumira, Lugazi and all Central Uganda directly to buyers.
        <br><br>
        <span class="text-green-300">Obulimi bwaffe, Obulamu bwaffe.</span>
      </p>

      <div class="flex gap-4 mt-8">
        <a href="#sell" class="bg-green-600 px-6 py-3 rounded-xl font-bold">🌾 Sell Produce</a>
        <a href="#market" class="bg-white text-black px-6 py-3 rounded-xl font-bold">🛒 Browse Market</a>
      </div>
    </div>

  </div>
</section>

<!-- MARKET -->
<section id="market" class="py-20 bg-white">
  <div class="max-w-7xl mx-auto px-6">

    <h2 class="text-3xl font-bold mb-8">Buyer Marketplace</h2>

    <input id="search" onkeyup="searchItems()" placeholder="Search produce..."
      class="w-full md:w-1/2 border p-3 rounded-xl mb-6"/>

    <div id="marketGrid" class="grid md:grid-cols-4 gap-6">

      <div class="card bg-white border rounded-2xl shadow overflow-hidden">
        <img class="h-40 w-full object-cover"
        src="https://images.unsplash.com/photo-1603048297172-c92544798d5a"/>

        <div class="p-4">
          <h3 class="font-bold">Matooke</h3>
          <p class="text-sm text-gray-500">Kayunga</p>
          <p class="text-green-700 font-bold">UGX 2,500</p>
        </div>
      </div>

      <div class="card bg-white border rounded-2xl shadow overflow-hidden">
        <img class="h-40 w-full object-cover"
        src="https://images.unsplash.com/photo-1542838132-92c53300491e"/>

        <div class="p-4">
          <h3 class="font-bold">Vegetables</h3>
          <p class="text-sm text-gray-500">Mukono</p>
          <p class="text-green-700 font-bold">UGX 3,000</p>
        </div>
      </div>

      <div class="card bg-white border rounded-2xl shadow overflow-hidden">
        <img class="h-40 w-full object-cover"
        src="https://images.unsplash.com/photo-1518977676601-b53f82aba655"/>

        <div class="p-4">
          <h3 class="font-bold">Cassava</h3>
          <p class="text-sm text-gray-500">Kangulumira</p>
          <p class="text-green-700 font-bold">UGX 1,800</p>
        </div>
      </div>

      <div class="card bg-white border rounded-2xl shadow overflow-hidden">
        <img class="h-40 w-full object-cover"
        src="https://images.unsplash.com/photo-1563565375-f3fdfdbefa83"/>

        <div class="p-4">
          <h3 class="font-bold">Eggs</h3>
          <p class="text-sm text-gray-500">Lugazi</p>
          <p class="text-green-700 font-bold">UGX 11,000</p>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- SELL -->
<section id="sell" class="py-20 bg-gray-50">
  <div class="max-w-5xl mx-auto px-6">

    <h2 class="text-3xl font-bold mb-6">Farmer Seller Dashboard</h2>

    <form id="form" class="bg-white p-6 rounded-2xl shadow space-y-4">

      <input id="name" class="w-full border p-3 rounded-xl" placeholder="Product Name">
      <input id="qty" class="w-full border p-3 rounded-xl" placeholder="Quantity">
      <input id="price" class="w-full border p-3 rounded-xl" placeholder="Price">
      <input id="loc" class="w-full border p-3 rounded-xl" placeholder="Location">

      <button class="w-full bg-green-600 text-white p-3 rounded-xl font-bold">
        Post Produce
      </button>

    </form>

    <div id="listings" class="mt-10 space-y-4"></div>

  </div>
</section>

<!-- ADS -->
<section id="ads" class="py-20 bg-white">
  <div class="max-w-7xl mx-auto px-6">

    <h2 class="text-3xl font-bold mb-10">Advertise Your Business</h2>

    <div class="grid md:grid-cols-3 gap-6">

      <div class="border p-6 rounded-2xl">
        <h3 class="font-bold text-xl">Starter</h3>
        <p class="text-green-700 font-bold text-2xl">UGX 50K</p>
      </div>

      <div class="border p-6 rounded-2xl bg-green-50">
        <h3 class="font-bold text-xl">Pro</h3>
        <p class="text-green-700 font-bold text-2xl">UGX 150K</p>
      </div>

      <div class="border p-6 rounded-2xl">
        <h3 class="font-bold text-xl">Enterprise</h3>
        <p class="text-green-700 font-bold text-2xl">Custom</p>
      </div>

    </div>

  </div>
</section>

<!-- TESTIMONIALS -->
<section class="py-20 bg-gray-50">
  <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-3 gap-6">

    <div class="bg-white p-6 rounded-2xl">
      “Nfunye sente mangu nnyo okuva ku Matooke.”
    </div>

    <div class="bg-white p-6 rounded-2xl">
      “Fresh vegetables direct from farmers.”
    </div>

    <div class="bg-white p-6 rounded-2xl">
      “Very easy even on phone.”
    </div>

  </div>
</section>

<!-- LOCATIONS -->
<section id="locations" class="py-20 bg-green-700 text-white text-center">
  <h2 class="text-3xl font-bold mb-6">Serving Central Uganda</h2>

  <div class="flex flex-wrap justify-center gap-3">
    <span class="bg-white/20 px-4 py-2 rounded-xl">Kayunga</span>
    <span class="bg-white/20 px-4 py-2 rounded-xl">Mukono</span>
    <span class="bg-white/20 px-4 py-2 rounded-xl">Lugazi</span>
    <span class="bg-white/20 px-4 py-2 rounded-xl">Kangulumira</span>
  </div>
</section>

<!-- FOOTER -->
<footer class="bg-black text-white text-center py-10">
  Kyalo Fresh © 2026 • Obulimi bwaffe, Obulamu bwaffe
</footer>

<!-- WHATSAPP -->
<a href="https://wa.me/256700000000"
class="fixed bottom-6 right-6 bg-green-500 text-white w-14 h-14 flex items-center justify-center rounded-full text-2xl">
💬
</a>

<script>

function toggleDark(){
  document.body.classList.toggle("bg-gray-900");
  document.body.classList.toggle("text-white");
}

document.getElementById("form").addEventListener("submit", function(e){
  e.preventDefault();

  const n = name.value;
  const q = qty.value;
  const p = price.value;
  const l = loc.value;

  const div = document.createElement("div");
  div.className = "bg-white p-4 rounded-xl shadow";
  div.innerHTML = `<b>${n}</b><br>${q} • ${l}<br><span class='text-green-700 font-bold'>${p}</span>`;

  listings.prepend(div);

  this.reset();
});

function searchItems(){
  let input = document.getElementById("search").value.toLowerCase();
  let cards = document.querySelectorAll("#marketGrid > div");

  cards.forEach(c=>{
    c.style.display = c.innerText.toLowerCase().includes(input) ? "block" : "none";
  });
}

</script>

</body>
</html>
