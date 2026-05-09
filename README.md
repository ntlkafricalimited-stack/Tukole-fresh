# Tukole-fresh
Reaching all central farmers

<html lang="en" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Tukole Fresh - Fresh from Our Villages to Your Kitchen</title>

  <script src="https://cdn.tailwindcss.com"></script>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

  <style>
    body{
      font-family: 'Inter', sans-serif;
    }

    .hero-bg{
      background:
      linear-gradient(to right, rgba(0,0,0,0.75), rgba(0,0,0,0.45)),
      url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1600&auto=format&fit=crop');
      background-size: cover;
      background-position: center;
    }

    .glass{
      backdrop-filter: blur(10px);
      background: rgba(255,255,255,0.08);
    }

    .card-hover{
      transition: all 0.3s ease;
    }

    .card-hover:hover{
      transform: translateY(-6px);
    }

    .dark-mode{
      background:#0f172a;
      color:white;
    }

    .dark-mode .bg-white{
      background:#1e293b !important;
      color:white !important;
    }

    .dark-mode .text-gray-700,
    .dark-mode .text-gray-600,
    .dark-mode .text-gray-500{
      color:#e2e8f0 !important;
    }

    .dark-mode input,
    .dark-mode select,
    .dark-mode textarea{
      background:#334155;
      color:white;
      border-color:#475569;
    }
  </style>
</head>

<body class="bg-gray-50 text-gray-800">

  <!-- NAVBAR -->
  <nav class="fixed top-0 w-full z-50 bg-white/95 shadow-sm backdrop-blur-md">
    <div class="max-w-7xl mx-auto px-4 py-3 flex items-center justify-between">

      <div class="flex items-center gap-3">
        <div class="w-11 h-11 rounded-full bg-green-600 flex items-center justify-center text-white font-bold text-xl">
          K
        </div>

        <div>
          <h1 class="font-extrabold text-xl text-green-700">Kyalo Fresh</h1>
          <p class="text-xs text-gray-500">Obulimi bwaffe, Obulamu bwaffe</p>
        </div>
      </div>

      <div class="hidden md:flex gap-8 font-medium">
        <a href="#market" class="hover:text-green-700">Market</a>
        <a href="#sell" class="hover:text-green-700">Sell Produce</a>
        <a href="#ads" class="hover:text-green-700">Advertise</a>
        <a href="#locations" class="hover:text-green-700">Locations</a>
      </div>

      <div class="flex items-center gap-3">
        <button onclick="toggleDarkMode()" class="bg-gray-100 px-4 py-2 rounded-full text-sm hover:bg-gray-200">
          🌙
        </button>

        <a href="https://wa.me/256700000000"
          class="bg-green-600 hover:bg-green-700 text-white px-5 py-2 rounded-full font-semibold shadow-lg">
          WhatsApp
        </a>
      </div>

    </div>
  </nav>

  <!-- HERO -->
  <section class="hero-bg min-h-screen flex items-center pt-24">
    <div class="max-w-7xl mx-auto px-6 grid lg:grid-cols-2 gap-12 items-center">

      <div>
        <div class="inline-block bg-orange-500 text-white px-4 py-2 rounded-full text-sm font-semibold mb-6">
          Central Uganda Digital Farmers Marketplace
        </div>

        <h1 class="text-5xl md:text-6xl font-extrabold text-white leading-tight mb-6">
          Sell Your Harvest Faster.
          <span class="text-green-400">
            Buy Fresh Produce Directly from Farmers.
          </span>
        </h1>

        <p class="text-lg text-gray-200 leading-relaxed mb-8">
          Connecting farmers from Ndese, Kayunga, Kangulumira, Mukono, Lugazi,
          Kalagi, Buikwe and all Central Uganda directly to homes, markets,
          restaurants and businesses.
        </p>

        <div class="flex flex-wrap gap-4">
          <a href="#sell"
            class="bg-green-600 hover:bg-green-700 text-white px-8 py-4 rounded-2xl font-bold text-lg shadow-xl">
            🌾 Post Produce
          </a>

          <a href="#market"
            class="bg-white text-gray-800 px-8 py-4 rounded-2xl font-bold text-lg shadow-xl hover:bg-gray-100">
            🛒 Browse Market
          </a>
        </div>

        <div class="flex flex-wrap gap-5 mt-10 text-white">
          <div class="glass px-5 py-4 rounded-2xl">
            <h3 class="text-3xl font-bold">2,500+</h3>
            <p>Farmers</p>
          </div>

          <div class="glass px-5 py-4 rounded-2xl">
            <h3 class="text-3xl font-bold">8+</h3>
            <p>Districts</p>
          </div>

          <div class="glass px-5 py-4 rounded-2xl">
            <h3 class="text-3xl font-bold">24/7</h3>
            <p>Marketplace</p>
          </div>
        </div>
      </div>

      <!-- HERO CARD -->
      <div class="bg-white rounded-3xl shadow-2xl p-8">

        <div class="flex items-center justify-between mb-6">
          <div>
            <h3 class="font-bold text-2xl text-green-700">Today's Fresh Listings</h3>
            <p class="text-gray-500">Live from our villages</p>
          </div>

          <div class="bg-green-100 text-green-700 px-4 py-2 rounded-full text-sm font-bold">
            LIVE
          </div>
        </div>

        <div class="space-y-4">

          <div class="flex items-center gap-4 p-4 rounded-2xl bg-gray-50">
            <img src="https://images.unsplash.com/photo-1528825871115-3581a5387919?q=80&w=400&auto=format&fit=crop"
              class="w-20 h-20 rounded-xl object-cover">

            <div class="flex-1">
              <h4 class="font-bold">Fresh Matooke</h4>
              <p class="text-sm text-gray-500">Kayunga • 500kg Available</p>
            </div>

            <div class="text-right">
              <h3 class="font-bold text-green-700">UGX 2,500</h3>
              <p class="text-xs">per bunch</p>
            </div>
          </div>

          <div class="flex items-center gap-4 p-4 rounded-2xl bg-gray-50">
            <img src="https://images.unsplash.com/photo-1518977676601-b53f82aba655?q=80&w=400&auto=format&fit=crop"
              class="w-20 h-20 rounded-xl object-cover">

            <div class="flex-1">
              <h4 class="font-bold">Organic Tomatoes</h4>
              <p class="text-sm text-gray-500">Mukono • 200kg</p>
            </div>

            <div class="text-right">
              <h3 class="font-bold text-green-700">UGX 3,000</h3>
              <p class="text-xs">per kg</p>
            </div>
          </div>

          <div class="flex items-center gap-4 p-4 rounded-2xl bg-gray-50">
            <img src="https://images.unsplash.com/photo-1563565375-f3fdfdbefa83?q=80&w=400&auto=format&fit=crop"
              class="w-20 h-20 rounded-xl object-cover">

            <div class="flex-1">
              <h4 class="font-bold">Fresh Eggs</h4>
              <p class="text-sm text-gray-500">Lugazi • 50 Trays</p>
            </div>

            <div class="text-right">
              <h3 class="font-bold text-orange-600">UGX 11,000</h3>
              <p class="text-xs">per tray</p>
            </div>
          </div>

        </div>

      </div>

    </div>
  </section>

  <!-- SEARCH -->
  <section id="market" class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-6">

      <div class="text-center mb-12">
        <h2 class="text-4xl font-extrabold mb-4">
          Buyer Marketplace
        </h2>

        <p class="text-gray-600 max-w-2xl mx-auto">
          Buy directly from trusted farmers across Central Uganda.
        </p>
      </div>

      <div class="grid md:grid-cols-4 gap-4 mb-10">

        <input type="text"
          id="searchInput"
          placeholder="Search produce..."
          class="border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-green-600">

        <select id="locationFilter"
          class="border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-green-600">
          <option value="">All Locations</option>
          <option>Kayunga</option>
          <option>Kangulumira</option>
          <option>Mukono</option>
          <option>Kalagi</option>
          <option>Lugazi</option>
          <option>Ndese</option>
        </select>

        <select class="border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-green-600">
          <option>All Products</option>
          <option>Vegetables</option>
          <option>Fruits</option>
          <option>Eggs</option>
          <option>Tubers</option>
        </select>

        <button
          class="bg-green-600 hover:bg-green-700 text-white rounded-2xl font-bold text-lg">
          Search Market
        </button>

      </div>

      <!-- PRODUCT GRID -->
      <div id="productGrid" class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">

        <!-- CARD -->
        <div class="bg-white rounded-3xl shadow-lg overflow-hidden card-hover border">
          <img src="https://images.unsplash.com/photo-1603048297172-c92544798d5a?q=80&w=600&auto=format&fit=crop"
            class="h-52 w-full object-cover">

          <div class="p-6">
            <div class="flex justify-between items-start mb-3">
              <h3 class="font-bold text-xl">Matooke</h3>
              <span class="bg-green-100 text-green-700 text-xs px-3 py-1 rounded-full">
                Fresh
              </span>
            </div>

            <p class="text-gray-500 mb-3">Kayunga</p>

            <div class="flex justify-between items-center mb-5">
              <h2 class="font-extrabold text-2xl text-green-700">
                UGX 2,500
              </h2>

              <span class="text-sm text-gray-500">
                per bunch
              </span>
            </div>

            <button
              class="w-full bg-green-600 hover:bg-green-700 text-white py-3 rounded-2xl font-bold">
              Order on WhatsApp
            </button>
          </div>
        </div>

        <!-- CARD -->
        <div class="bg-white rounded-3xl shadow-lg overflow-hidden card-hover border">
          <img src="https://images.unsplash.com/photo-1542838132-92c53300491e?q=80&w=600&auto=format&fit=crop"
            class="h-52 w-full object-cover">

          <div class="p-6">
            <div class="flex justify-between items-start mb-3">
              <h3 class="font-bold text-xl">Vegetables</h3>
              <span class="bg-orange-100 text-orange-700 text-xs px-3 py-1 rounded-full">
                Organic
              </span>
            </div>

            <p class="text-gray-500 mb-3">Mukono</p>

            <div class="flex justify-between items-center mb-5">
              <h2 class="font-extrabold text-2xl text-green-700">
                UGX 3,500
              </h2>

              <span class="text-sm text-gray-500">
                per kg
              </span>
            </div>

            <button
              class="w-full bg-green-600 hover:bg-green-700 text-white py-3 rounded-2xl font-bold">
              Order on WhatsApp
            </button>
          </div>
        </div>

        <!-- CARD -->
        <div class="bg-white rounded-3xl shadow-lg overflow-hidden card-hover border">
          <img src="https://images.unsplash.com/photo-1518977676601-b53f82aba655?q=80&w=600&auto=format&fit=crop"
            class="h-52 w-full object-cover">

          <div class="p-6">
            <div class="flex justify-between items-start mb-3">
              <h3 class="font-bold text-xl">Cassava</h3>
              <span class="bg-green-100 text-green-700 text-xs px-3 py-1 rounded-full">
                Bulk
              </span>
            </div>

            <p class="text-gray-500 mb-3">Kangulumira</p>

            <div class="flex justify-between items-center mb-5">
              <h2 class="font-extrabold text-2xl text-green-700">
                UGX 1,800
              </h2>

              <span class="text-sm text-gray-500">
                per kg
              </span>
            </div>

            <button
              class="w-full bg-green-600 hover:bg-green-700 text-white py-3 rounded-2xl font-bold">
              Order on WhatsApp
            </button>
          </div>
        </div>

        <!-- CARD -->
        <div class="bg-white rounded-3xl shadow-lg overflow-hidden card-hover border">
          <img src="https://images.unsplash.com/photo-1563565375-f3fdfdbefa83?q=80&w=600&auto=format&fit=crop"
            class="h-52 w-full object-cover">

          <div class="p-6">
            <div class="flex justify-between items-start mb-3">
              <h3 class="font-bold text-xl">Eggs</h3>
              <span class="bg-yellow-100 text-yellow-700 text-xs px-3 py-1 rounded-full">
                Farm Fresh
              </span>
            </div>

            <p class="text-gray-500 mb-3">Lugazi</p>

            <div class="flex justify-between items-center mb-5">
              <h2 class="font-extrabold text-2xl text-green-700">
                UGX 11,000
              </h2>

              <span class="text-sm text-gray-500">
                per tray
              </span>
            </div>

            <button
              class="w-full bg-green-600 hover:bg-green-700 text-white py-3 rounded-2xl font-bold">
              Order on WhatsApp
            </button>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- SELL SECTION -->
  <section id="sell" class="py-20 bg-green-50">
    <div class="max-w-7xl mx-auto px-6 grid lg:grid-cols-2 gap-14">

      <div>
        <h2 class="text-4xl font-extrabold mb-5">
          Farmer Seller Dashboard
        </h2>

        <p class="text-gray-600 mb-10">
          Post your produce quickly and connect directly with buyers.
        </p>

        <form id="produceForm" class="bg-white rounded-3xl shadow-xl p-8 space-y-5">

          <input type="text"
            id="productName"
            placeholder="Product Name"
            class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-green-600"
            required>

          <input type="text"
            id="quantity"
            placeholder="Quantity Available"
            class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-green-600"
            required>

          <input type="text"
            id="price"
            placeholder="Price per kg / bunch"
            class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-green-600"
            required>

          <select id="location"
            class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-green-600">

            <option>Choose Location</option>
            <option>Kayunga</option>
            <option>Mukono</option>
            <option>Kangulumira</option>
            <option>Kalagi</option>
            <option>Lugazi</option>
            <option>Ndese</option>
          </select>

          <input type="text"
            placeholder="Phone Contact"
            class="w-full border border-gray-300 rounded-2xl px-5 py-4 outline-none focus:border-green-600">

          <div class="border-2 border-dashed border-gray-300 rounded-2xl p-8 text-center">
            📸 Photo Upload Placeholder
          </div>

          <button
            class="w-full bg-green-600 hover:bg-green-700 text-white py-4 rounded-2xl font-bold text-lg">
            Post Produce
          </button>

        </form>
      </div>

      <!-- MY LISTINGS -->
      <div>
        <div class="flex justify-between items-center mb-6">
          <div>
            <h2 class="text-3xl font-extrabold">My Listings</h2>
            <p class="text-gray-600">Your posted produce appears here.</p>
          </div>

          <div class="bg-orange-500 text-white px-4 py-2 rounded-full text-sm font-bold">
            Farmer Mode
          </div>
        </div>

        <div id="myListings" class="space-y-5">

          <div class="bg-white p-6 rounded-3xl shadow-md">
            <div class="flex justify-between">
              <div>
                <h3 class="font-bold text-xl">Tomatoes</h3>
                <p class="text-gray-500">Mukono • 120kg</p>
              </div>

              <div class="text-right">
                <h3 class="font-bold text-green-700">UGX 3,000</h3>
                <p class="text-sm text-gray-500">per kg</p>
              </div>
            </div>
          </div>

        </div>

      </div>
    </div>
  </section>

  <!-- HOW IT WORKS -->
  <section class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-6 text-center">

      <h2 class="text-4xl font-extrabold mb-4">
        How Kyalo Fresh Works
      </h2>

      <p class="text-gray-600 mb-14">
        Easy for every farmer and every buyer.
      </p>

      <div class="grid md:grid-cols-4 gap-8">

        <div class="bg-green-50 p-8 rounded-3xl">
          <div class="text-5xl mb-5">🌾</div>
          <h3 class="font-bold text-xl mb-3">1. Post Produce</h3>
          <p class="text-gray-600">
            Farmers upload available produce and prices.
          </p>
        </div>

        <div class="bg-orange-50 p-8 rounded-3xl">
          <div class="text-5xl mb-5">📍</div>
          <h3 class="font-bold text-xl mb-3">2. Buyers Search</h3>
          <p class="text-gray-600">
            Buyers filter by product, location and pricing.
          </p>
        </div>

        <div class="bg-green-50 p-8 rounded-3xl">
          <div class="text-5xl mb-5">💬</div>
          <h3 class="font-bold text-xl mb-3">3. Connect</h3>
          <p class="text-gray-600">
            Direct WhatsApp contact between farmer and buyer.
          </p>
        </div>

        <div class="bg-orange-50 p-8 rounded-3xl">
          <div class="text-5xl mb-5">🚚</div>
          <h3 class="font-bold text-xl mb-3">4. Deliver</h3>
          <p class="text-gray-600">
            Produce delivered quickly and fresh.
          </p>
        </div>

      </div>
    </div>
  </section>

  <!-- ADS -->
  <section id="ads" class="py-20 bg-gray-100">
    <div class="max-w-7xl mx-auto px-6">

      <div class="text-center mb-14">
        <h2 class="text-4xl font-extrabold mb-4">
          Advertise Your Business
        </h2>

        <p class="text-gray-600">
          Reach thousands of farmers and produce buyers daily.
        </p>
      </div>

      <div class="grid md:grid-cols-3 gap-8">

        <div class="bg-white p-8 rounded-3xl shadow-lg">
          <h3 class="font-bold text-2xl mb-4">Starter</h3>
          <h2 class="text-5xl font-extrabold text-green-700 mb-6">
            UGX 50K
          </h2>

          <ul class="space-y-3 text-gray-600 mb-8">
            <li>✔ Agro-vet Listing</li>
            <li>✔ Business Profile</li>
            <li>✔ WhatsApp Contact</li>
          </ul>

          <button class="w-full bg-green-600 text-white py-3 rounded-2xl font-bold">
            Get Started
          </button>
        </div>

        <div class="bg-green-700 text-white p-8 rounded-3xl shadow-2xl scale-105">
          <div class="bg-orange-400 inline-block px-4 py-2 rounded-full text-sm font-bold mb-5">
            MOST POPULAR
          </div>

          <h3 class="font-bold text-2xl mb-4">Business Pro</h3>

          <h2 class="text-5xl font-extrabold mb-6">
            UGX 150K
          </h2>

          <ul class="space-y-3 mb-8">
            <li>✔ Featured Placement</li>
            <li>✔ Supplier Promotion</li>
            <li>✔ WhatsApp Leads</li>
            <li>✔ Weekly Boost</li>
          </ul>

          <button class="w-full bg-orange-500 py-3 rounded-2xl font-bold">
            Advertise Now
          </button>
        </div>

        <div class="bg-white p-8 rounded-3xl shadow-lg">
          <h3 class="font-bold text-2xl mb-4">Enterprise</h3>
          <h2 class="text-5xl font-extrabold text-green-700 mb-6">
            Custom
          </h2>

          <ul class="space-y-3 text-gray-600 mb-8">
            <li>✔ Millers & Distributors</li>
            <li>✔ Transport Partners</li>
            <li>✔ Priority Visibility</li>
          </ul>

          <button class="w-full bg-green-600 text-white py-3 rounded-2xl font-bold">
            Contact Team
          </button>
        </div>

      </div>
    </div>
  </section>

  <!-- TESTIMONIALS -->
  <section class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-6">

      <div class="text-center mb-14">
        <h2 class="text-4xl font-extrabold mb-4">
          Trusted by Farmers & Buyers
        </h2>

        <p class="text-gray-600">
          Real stories from Central Uganda.
        </p>
      </div>

      <div class="grid md:grid-cols-3 gap-8">

        <div class="bg-green-50 p-8 rounded-3xl">
          <p class="text-gray-700 mb-6">
            “Kyalo Fresh helped me sell my matooke faster without middlemen.
            Nfunye sente mangu nnyo.”
          </p>

          <div>
            <h4 class="font-bold">Sarah N.</h4>
            <p class="text-gray-500">Farmer • Kayunga</p>
          </div>
        </div>

        <div class="bg-orange-50 p-8 rounded-3xl">
          <p class="text-gray-700 mb-6">
            “Fresh vegetables delivered directly from Mukono farms.
            Very reliable platform.”
          </p>

          <div>
            <h4 class="font-bold">Brian K.</h4>
            <p class="text-gray-500">Restaurant Owner • Kampala</p>
          </div>
        </div>

        <div class="bg-green-50 p-8 rounded-3xl">
          <p class="text-gray-700 mb-6">
            “Easy to use even on phone. Farmers can post produce quickly.”
          </p>

          <div>
            <h4 class="font-bold">Mariam T.</h4>
            <p class="text-gray-500">Egg Supplier • Lugazi</p>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- LOCATIONS -->
  <section id="locations" class="py-20 bg-green-700 text-white">
    <div class="max-w-7xl mx-auto px-6 text-center">

      <h2 class="text-4xl font-extrabold mb-5">
        Serving All Central Uganda
      </h2>

      <p class="max-w-3xl mx-auto text-green-100 mb-10">
        Kyalo Fresh proudly connects farmers and buyers across:
      </p>

      <div class="flex flex-wrap justify-center gap-4">

        <div class="bg-white/10 px-6 py-4 rounded-2xl">Ndese</div>
        <div class="bg-white/10 px-6 py-4 rounded-2xl">Kangulumira</div>
        <div class="bg-white/10 px-6 py-4 rounded-2xl">Kayunga</div>
        <div class="bg-white/10 px-6 py-4 rounded-2xl">Mukono</div>
        <div class="bg-white/10 px-6 py-4 rounded-2xl">Kalagi</div>
        <div class="bg-white/10 px-6 py-4 rounded-2xl">Lugazi</div>
        <div class="bg-white/10 px-6 py-4 rounded-2xl">Buikwe</div>
        <div class="bg-white/10 px-6 py-4 rounded-2xl">Jinja Road Areas</div>

      </div>

    </div>
  </section>

  <!-- FOOTER -->
  <footer class="bg-gray-900 text-gray-300 py-14">
    <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-4 gap-10">

      <div>
        <h3 class="text-2xl font-extrabold text-white mb-4">
          Kyalo Fresh
        </h3>

        <p class="text-gray-400 leading-relaxed">
          Fresh from Our Villages to Your Kitchen.
          Building digital agriculture for Central Uganda.
        </p>
      </div>

      <div>
        <h4 class="font-bold text-white mb-4">Marketplace</h4>

        <ul class="space-y-2">
          <li>Buy Produce</li>
          <li>Sell Produce</li>
          <li>Farmer Accounts</li>
          <li>Bulk Orders</li>
        </ul>
      </div>

      <div>
        <h4 class="font-bold text-white mb-4">Locations</h4>

        <ul class="space-y-2">
          <li>Kayunga</li>
          <li>Mukono</li>
          <li>Lugazi</li>
          <li>Kangulumira</li>
        </ul>
      </div>

      <div>
        <h4 class="font-bold text-white mb-4">Contact</h4>

        <ul class="space-y-3">
          <li>📞 +256 745393259 </li>
          <li>✉ info@kyalofresh.com</li>
          <li>📍 Central Uganda</li>
        </ul>
      </div>

    </div>

    <div class="border-t border-gray-800 mt-12 pt-8 text-center text-gray-500">
      © 2026 tukole Fresh. All rights reserved.
    </div>
  </footer>

  <!-- FLOATING WHATSAPP -->
  <a href="https://wa.me/256700000000"
    class="fixed bottom-6 right-6 bg-green-500 hover:bg-green-600 text-white w-16 h-16 rounded-full flex items-center justify-center text-3xl shadow-2xl z-50">
    💬
  </a>

  <!-- JAVASCRIPT -->
  <script>

    // ADD LISTING
    const form = document.getElementById('produceForm');
    const listings = document.getElementById('myListings');

    form.addEventListener('submit', function(e){
      e.preventDefault();

      const product = document.getElementById('productName').value;
      const quantity = document.getElementById('quantity').value;
      const price = document.getElementById('price').value;
      const location = document.getElementById('location').value;

      const card = document.createElement('div');

      card.className = "bg-white p-6 rounded-3xl shadow-md";

      card.innerHTML = `
        <div class="flex justify-between">
          <div>
            <h3 class="font-bold text-xl">${product}</h3>
            <p class="text-gray-500">${location} • ${quantity}</p>
          </div>

          <div class="text-right">
            <h3 class="font-bold text-green-700">${price}</h3>
            <p class="text-sm text-gray-500">new listing</p>
          </div>
        </div>
      `;

      listings.prepend(card);

      form.reset();

      alert("Produce posted successfully!");
    });

    // DARK MODE
    function toggleDarkMode(){
      document.body.classList.toggle('dark-mode');
    }

    // SEARCH FILTER
    const searchInput = document.getElementById('searchInput');

    searchInput.addEventListener('keyup', function(){
      const filter = searchInput.value.toLowerCase();
      const cards = document.querySelectorAll('#productGrid > div');

      cards.forEach(card => {
        const text = card.innerText.toLowerCase();

        if(text.includes(filter)){
          card.style.display = "block";
        } else {
          card.style.display = "none";
        }
      });
    });

  </script>

</body>
</html>
