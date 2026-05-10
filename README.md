<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Kyalo Fresh - Obulimi bwaffe</title>

  <script src="https://cdn.tailwindcss.com"></script>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

  <style>

    body{
      font-family:'Inter',sans-serif;
      overflow-x:hidden;
      background:#f8faf7;
    }

    .hero-bg{
      background:
      linear-gradient(to top, rgba(0,0,0,.75), rgba(0,0,0,.35)),
      url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1600&auto=format&fit=crop');
      background-size:cover;
      background-position:center;
    }

    .glass{
      backdrop-filter:blur(12px);
      background:rgba(255,255,255,.12);
      border:1px solid rgba(255,255,255,.12);
    }

    .card{
      transition:.3s ease;
    }

    .card:hover{
      transform:translateY(-8px);
    }

    .village-pattern{
      background-image:
      radial-gradient(rgba(34,197,94,.06) 2px, transparent 2px);
      background-size:24px 24px;
    }

  </style>
</head>

<body class="text-gray-800">

<!-- TOP BAR -->
<div class="bg-green-900 text-white text-sm py-2 px-4 text-center">
  🌾 Tukuyunga ku balimi ba Central Uganda • Fresh Produce Daily
</div>

<!-- NAVBAR -->
<header class="fixed top-0 left-0 w-full z-50 bg-white/95 backdrop-blur-md shadow-sm">

  <div class="max-w-7xl mx-auto px-4 sm:px-6">

    <div class="flex items-center justify-between h-20">

      <!-- LOGO -->
      <div class="flex items-center gap-3">

        <div class="w-12 h-12 rounded-full bg-gradient-to-br from-green-600 to-orange-500 flex items-center justify-center text-white font-extrabold text-xl shadow-lg">
          🌾
        </div>

        <div>
          <h1 class="font-extrabold text-2xl text-green-800">
            Kyalo Fresh
          </h1>

          <p class="text-xs text-gray-500">
            Obulimi bwaffe • Fresh okuva mu kyalo
          </p>
        </div>

      </div>

      <!-- MENU -->
      <nav class="hidden lg:flex items-center gap-8 font-semibold">

        <a href="#market" class="hover:text-green-700 transition">
          Market
        </a>

        <a href="#farmers" class="hover:text-green-700 transition">
          Farmers
        </a>

        <a href="#ads" class="hover:text-green-700 transition">
          Business Ads
        </a>

        <a href="#locations" class="hover:text-green-700 transition">
          Locations
        </a>

      </nav>

      <!-- ACTION -->
      <a href="https://wa.me/256700000000"
      class="bg-green-600 hover:bg-green-700 text-white px-5 py-3 rounded-full font-bold shadow-lg transition">

        WhatsApp

      </a>

    </div>

  </div>

</header>

<!-- HERO -->
<section class="hero-bg min-h-screen flex items-center pt-28">

  <div class="max-w-7xl mx-auto px-6 w-full">

    <div class="grid lg:grid-cols-2 gap-16 items-center">

      <!-- LEFT -->
      <div>

        <div class="inline-flex items-center gap-2 glass text-white px-5 py-3 rounded-full mb-8">
          🚜 Uganda Rural Digital Marketplace
        </div>

        <h1 class="text-5xl md:text-7xl font-extrabold text-white leading-tight">

          Gulisa
          <span class="text-green-400">
            Ebirime Byo
          </span>
          Mangu.

        </h1>

        <h2 class="text-2xl md:text-3xl text-orange-300 font-bold mt-5">
          Fresh okuva mu byalo byaffe straight to your kitchen.
        </h2>

        <p class="text-lg text-gray-200 leading-relaxed mt-8 max-w-2xl">

          Kyalo Fresh helps farmers okuva e Kayunga,
          Mukono, Lugazi, Kalagi, Kangulumira ne Central Uganda
          okutunda ebirime byabwe directly eri buyers, restaurants,
          markets ne homes.

        </p>

        <!-- BUTTONS -->
        <div class="flex flex-col sm:flex-row gap-5 mt-10">

          <a href="#sell"
          class="bg-green-600 hover:bg-green-700 text-white px-8 py-5 rounded-2xl text-lg font-bold shadow-2xl text-center">

            🌾 Teeka Ebirime

          </a>

          <a href="#market"
          class="bg-white hover:bg-gray-100 text-gray-900 px-8 py-5 rounded-2xl text-lg font-bold shadow-2xl text-center">

            🛒 Gula Produce

          </a>

        </div>

        <!-- STATS -->
        <div class="grid grid-cols-3 gap-4 mt-12">

          <div class="glass p-5 rounded-2xl text-center">
            <h3 class="text-3xl font-extrabold text-white">
              2,500+
            </h3>

            <p class="text-sm text-gray-200">
              Farmers
            </p>
          </div>

          <div class="glass p-5 rounded-2xl text-center">
            <h3 class="text-3xl font-extrabold text-white">
              24/7
            </h3>

            <p class="text-sm text-gray-200">
              Market
            </p>
          </div>

          <div class="glass p-5 rounded-2xl text-center">
            <h3 class="text-3xl font-extrabold text-white">
              8+
            </h3>

            <p class="text-sm text-gray-200">
              Districts
            </p>
          </div>

        </div>

      </div>

      <!-- RIGHT -->
      <div class="relative">

        <div class="bg-white rounded-[2rem] shadow-2xl p-7">

          <div class="flex items-center justify-between mb-8">

            <div>
              <h3 class="text-2xl font-extrabold text-green-800">
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

            <!-- ITEM -->
            <div class="flex items-center gap-4 bg-green-50 p-4 rounded-2xl card">

              <img src="https://images.unsplash.com/photo-1603048297172-c92544798d5a?q=80&w=600&auto=format&fit=crop"
              class="w-24 h-24 rounded-2xl object-cover">

              <div class="flex-1">

                <h4 class="font-extrabold text-lg">
                  Matooke
                </h4>

                <p class="text-gray-500">
                  Kayunga • 500 Bunches
                </p>

                <div class="flex items-center gap-2 mt-2">
                  <span class="bg-green-200 text-green-800 text-xs px-3 py-1 rounded-full font-bold">
                    Fresh Today
                  </span>
                </div>

              </div>

              <div class="text-right">

                <h3 class="font-extrabold text-2xl text-green-700">
                  UGX 2,500
                </h3>

                <p class="text-sm text-gray-500">
                  per bunch
                </p>

              </div>

            </div>

            <!-- ITEM -->
            <div class="flex items-center gap-4 bg-orange-50 p-4 rounded-2xl card">

              <img src="https://images.unsplash.com/photo-1542838132-92c53300491e?q=80&w=600&auto=format&fit=crop"
              class="w-24 h-24 rounded-2xl object-cover">

              <div class="flex-1">

                <h4 class="font-extrabold text-lg">
                  Vegetables
                </h4>

                <p class="text-gray-500">
                  Mukono • 300kg
                </p>

                <div class="flex items-center gap-2 mt-2">
                  <span class="bg-orange-200 text-orange-800 text-xs px-3 py-1 rounded-full font-bold">
                    Organic
                  </span>
                </div>

              </div>

              <div class="text-right">

                <h3 class="font-extrabold text-2xl text-orange-600">
                  UGX 3,000
                </h3>

                <p class="text-sm text-gray-500">
                  per kg
                </p>

              </div>

            </div>

          </div>

        </div>

        <!-- FLOAT CARD -->
        <div class="hidden lg:block absolute -bottom-8 -left-8 bg-orange-500 text-white p-6 rounded-3xl shadow-2xl">

          <h3 class="text-3xl font-extrabold">
            98%
          </h3>

          <p class="font-medium">
            Faster farmer sales
          </p>

        </div>

      </div>

    </div>

  </div>

</section>

<!-- MARKETPLACE -->
<section id="market" class="py-24 village-pattern">

  <div class="max-w-7xl mx-auto px-6">

    <div class="text-center mb-16">

      <h2 class="text-5xl font-extrabold text-green-800">
        Buyer Marketplace
      </h2>

      <p class="text-gray-600 mt-5 text-lg max-w-2xl mx-auto">
        Buy fresh produce directly okuva eri abalimi.
      </p>

    </div>

    <!-- SEARCH -->
    <div class="bg-white rounded-3xl shadow-xl p-6 mb-14">

      <div class="grid lg:grid-cols-4 gap-5">

        <input type="text"
        placeholder="🔍 Search produce..."
        class="border border-gray-200 rounded-2xl px-5 py-4 outline-none focus:border-green-600">

        <select class="border border-gray-200 rounded-2xl px-5 py-4 outline-none focus:border-green-600">
          <option>📍 All Locations</option>
          <option>Kayunga</option>
          <option>Mukono</option>
          <option>Lugazi</option>
        </select>

        <select class="border border-gray-200 rounded-2xl px-5 py-4 outline-none focus:border-green-600">
          <option>🌾 All Products</option>
          <option>Matooke</option>
          <option>Vegetables</option>
        </select>

        <button class="bg-green-600 hover:bg-green-700 text-white rounded-2xl font-bold text-lg">
          Search Market
        </button>

      </div>

    </div>

    <!-- GRID -->
    <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-8">

      <div class="bg-white rounded-3xl shadow-lg overflow-hidden card">

        <img src="https://images.unsplash.com/photo-1603048297172-c92544798d5a?q=80&w=600&auto=format&fit=crop"
        class="h-56 w-full object-cover">

        <div class="p-6">

          <div class="flex justify-between items-start mb-4">

            <div>
              <h3 class="font-extrabold text-xl">
                Matooke
              </h3>

              <p class="text-gray-500">
                Kayunga
              </p>
            </div>

            <span class="bg-green-100 text-green-700 text-xs px-3 py-1 rounded-full font-bold">
              Fresh
            </span>

          </div>

          <div class="flex justify-between items-center mb-5">

            <h3 class="font-extrabold text-3xl text-green-700">
              UGX 2,500
            </h3>

            <span class="text-sm text-gray-500">
              per bunch
            </span>

          </div>

          <button class="w-full bg-green-600 hover:bg-green-700 text-white py-4 rounded-2xl font-bold">
            WhatsApp Order
          </button>

        </div>

      </div>

    </div>

  </div>

</section>

<!-- FOOTER -->
<footer class="bg-green-950 text-white py-16">

  <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-4 gap-10">

    <div>

      <h3 class="text-3xl font-extrabold mb-5">
        Kyalo Fresh
      </h3>

      <p class="text-green-200 leading-relaxed">
        Fresh okuva mu byalo byaffe.
      </p>

    </div>

    <div>

      <h4 class="font-bold text-xl mb-5">
        Marketplace
      </h4>

      <ul class="space-y-3 text-green-200">
        <li>Buy Produce</li>
        <li>Sell Produce</li>
        <li>Farmer Accounts</li>
      </ul>

    </div>

    <div>

      <h4 class="font-bold text-xl mb-5">
        Locations
      </h4>

      <ul class="space-y-3 text-green-200">
        <li>Kayunga</li>
        <li>Mukono</li>
        <li>Lugazi</li>
      </ul>

    </div>

    <div>

      <h4 class="font-bold text-xl mb-5">
        Contact
      </h4>

      <ul class="space-y-3 text-green-200">
        <li>📞 +256 700 000000</li>
        <li>📍 Central Uganda</li>
      </ul>

    </div>

  </div>

</footer>

<!-- FLOATING WHATSAPP -->
<a href="https://wa.me/256700000000"
class="fixed bottom-6 right-6 bg-green-500 hover:bg-green-600 text-white w-16 h-16 rounded-full flex items-center justify-center text-3xl shadow-2xl z-50">

💬

</a>

</body>
</html>
