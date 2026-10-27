
<html lang="hi" class="scroll-smooth">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mindo Pickles | घर जैसा स्वाद • 100% Traditional Handcrafted Pickles</title>
  
  <!-- Google Fonts: Playfair Display, Plus Jakarta Sans & Rozha One for Indian heritage typography -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Playfair+Display:ital,wght@0,600;0,700;0,800;0,900;1,600&family=Rozha+One&family=Yatra+One&display=swap" rel="stylesheet">
  
  <!-- Font Awesome 6 Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  
  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          colors: {
            brand: {
              cream: '#FCF8F1',
              creamlite: '#FFFDF9',
              gold: '#E5A93B',
              golddark: '#C8871E',
              green: '#184E34',
              greendark: '#0F3422',
              greenlight: '#E7F2EB',
              red: '#B82E24',
              redhover: '#9E241B',
              terracotta: '#D95B30',
              earth: '#281E19',
              muted: '#76685E'
            }
          },
          fontFamily: {
            sans: ['"Plus Jakarta Sans"', 'sans-serif'],
            serif: ['"Playfair Display"', 'serif'],
            heritage: ['"Rozha One"', 'serif'],
            hindi: ['"Yatra One"', 'cursive']
          },
          boxShadow: {
            'warm': '0 10px 30px -5px rgba(184, 46, 36, 0.12), 0 8px 10px -6px rgba(40, 30, 25, 0.06)',
            'card-hover': '0 20px 40px -10px rgba(24, 78, 52, 0.18)',
            'floating': '0 12px 35px rgba(15, 52, 34, 0.25)'
          }
        }
      }
    }
  </script>

  <style>
    /* Custom Scrollbar */
    ::-webkit-scrollbar {
      width: 7px;
    }
    ::-webkit-scrollbar-track {
      background: #F4EADA;
    }
    ::-webkit-scrollbar-thumb {
      background: #C8871E;
      border-radius: 4px;
    }

    /* Ambient Indian Royal Background texture */
    .bg-heritage-pattern {
      background-color: #FCF8F1;
      background-image: radial-gradient(#d4af37 0.65px, transparent 0.65px), radial-gradient(#184e34 0.65px, #FCF8F1 0.65px);
      background-size: 26px 26px;
      background-position: 0 0, 13px 13px;
      background-opacity: 0.15;
    }

    .shimmer-gold {
      background: linear-gradient(90deg, #E5A93B 0%, #FFF3CC 50%, #E5A93B 100%);
      background-size: 200% auto;
      color: transparent;
      -webkit-background-clip: text;
      animation: shimmer 5s linear infinite;
    }

    @keyframes shimmer {
      to { background-position: 200% center; }
    }

    /* Custom Glassmorphism */
    .glass-nav {
      background: rgba(252, 248, 241, 0.88);
      backdrop-filter: blur(14px);
      -webkit-backdrop-filter: blur(14px);
    }
    
    .glass-card {
      background: rgba(255, 255, 255, 0.85);
      backdrop-filter: blur(8px);
      border: 1px solid rgba(229, 169, 59, 0.2);
    }

    /* Floating micro animations */
    @keyframes floatGentle {
      0%, 100% { transform: translateY(0px) rotate(0deg); }
      50% { transform: translateY(-12px) rotate(3deg); }
    }
    .floating-ornament {
      animation: floatGentle 6s ease-in-out infinite;
    }
  </style>
</head>

<body class="bg-heritage-pattern text-brand-earth font-sans min-h-screen selection:bg-brand-gold selection:text-brand-greendark flex flex-col justify-between">

  <!-- TOP ANNOUNCEMENT BAR -->
  <div class="bg-brand-greendark text-brand-gold px-4 py-2 text-xs md:text-sm font-medium tracking-wide flex justify-center items-center gap-3 border-b border-brand-gold/30">
    <span class="inline-flex items-center gap-1.5"><i class="fa-solid fa-mortar-pestle text-brand-gold animate-pulse"></i> 100% Traditional Sun-Dried • Made in Pure Kachi Ghani Mustard Oil</span>
    <span class="hidden md:inline text-brand-creamlite/40">|</span>
    <span class="hidden md:inline text-brand-creamlite">📦 Free Fast Delivery on orders above ₹699</span>
  </div>

  <!-- NAVIGATION HEADER -->
  <header class="sticky top-0 z-40 glass-nav border-b border-brand-earth/10 transition-all duration-300">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
      
      <!-- Logo Branding -->
      <a href="#" class="flex items-center gap-3 group">
        <div class="w-12 h-12 rounded-2xl bg-gradient-to-tr from-brand-greendark to-brand-green flex items-center justify-center text-brand-gold shadow-md shadow-brand-green/20 group-hover:scale-105 transition-transform duration-300">
          <i class="fa-solid fa-jar text-2xl"></i>
        </div>
        <div class="flex flex-col">
          <span class="font-serif font-black text-2xl md:text-3xl tracking-tight text-brand-greendark leading-none">
            Mindo<span class="text-brand-red font-heritage">.</span>
          </span>
          <span class="font-hindi text-xs tracking-wider text-brand-golddark font-semibold mt-0.5">घर जैसा असली स्वाद</span>
        </div>
      </a>

      <!-- Desktop Links -->
      <nav class="hidden lg:flex items-center gap-8 font-medium text-brand-earth/80 text-sm tracking-wide">
        <a href="#pickles" class="hover:text-brand-red transition-colors flex items-center gap-1.5"><i class="fa-solid fa-pepper-hot text-brand-red/70 text-xs"></i> हमारे अचार (Shop)</a>
        <a href="#why-us" class="hover:text-brand-green transition-colors">Speciality</a>
        <a href="#ingredients" class="hover:text-brand-green transition-colors">Pure Spices</a>
        <a href="#reviews" class="hover:text-brand-green transition-colors">Reviews</a>
        <a href="#contact" class="hover:text-brand-green transition-colors">Contact</a>
      </nav>

      <!-- Right CTAs -->
      <div class="flex items-center gap-3 md:gap-4">
        <!-- Direct WhatsApp Quick Help -->
        <a href="https://wa.me/918383050500" target="_blank" class="hidden sm:inline-flex items-center gap-2 text-xs font-semibold px-3 py-2 rounded-full border border-brand-green/20 text-brand-green hover:bg-brand-greenlight transition">
          <i class="fa-brands fa-whatsapp text-emerald-600 text-base"></i>
          <span>Helpdesk</span>
        </a>

        <!-- Cart Trigger Button -->
        <button onclick="openCart()" class="relative bg-brand-green hover:bg-brand-greendark text-white px-4 md:px-5 py-2.5 rounded-full flex items-center gap-2.5 shadow-md shadow-brand-green/30 hover:shadow-lg transition-all transform active:scale-95 duration-200">
          <i class="fa-solid fa-basket-shopping text-sm md:text-base text-brand-gold"></i>
          <span class="font-bold text-xs md:text-sm tracking-wider uppercase">Cart</span>
          <span id="navCartBadge" class="bg-brand-red text-white text-[11px] font-black h-5 w-5 rounded-full flex items-center justify-center border-2 border-white">0</span>
        </button>
      </div>
    </div>
  </header>

  <!-- HERO SECTION -->
  <section class="relative overflow-hidden pt-12 pb-20 md:py-24 bg-gradient-to-b from-[#FFF9EE] via-[#FCF5E6] to-brand-cream border-b border-brand-earth/5">
    <!-- Floating Organic Food Icons in Background -->
    <div class="absolute top-10 left-[6%] text-brand-gold/25 text-5xl floating-ornament pointer-events-none select-none">🥭</div>
    <div class="absolute bottom-16 left-[10%] text-brand-red/25 text-4xl floating-ornament pointer-events-none select-none" style="animation-delay: 2s;">🌶️</div>
    <div class="absolute top-14 right-[8%] text-brand-green/20 text-5xl floating-ornament pointer-events-none select-none" style="animation-delay: 1.2s;">🍋</div>
    <div class="absolute bottom-20 right-[12%] text-brand-gold/30 text-4xl floating-ornament pointer-events-none select-none" style="animation-delay: 3s;">🫙</div>

    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
        
        <!-- Left Content -->
        <div class="lg:col-span-7 text-center lg:text-left space-y-6">
          
          <div class="inline-flex items-center gap-2 bg-gradient-to-r from-brand-green/10 to-brand-gold/15 border border-brand-green/20 px-4 py-1.5 rounded-full">
            <span class="flex h-2 w-2 rounded-full bg-emerald-600 animate-ping"></span>
            <span class="text-xs md:text-sm font-semibold tracking-wide text-brand-greendark font-hindi">100% शुद्ध सरसों तेल • बरनी में धूप-पका</span>
          </div>

          <h1 class="font-serif text-4xl sm:text-5xl xl:text-6xl text-brand-greendark font-black leading-[1.15] tracking-tight">
            घर जैसा असली स्वाद, <br class="hidden sm:inline">
            <span class="text-brand-red font-hindi">दादी-नानी</span> के प्यार से बना।
          </h1>

          <p class="text-base sm:text-lg text-brand-muted max-w-2xl mx-auto lg:mx-0 font-normal leading-relaxed">
            Mindo Pickles brings the legendary taste of traditional Northern Indian households right to your plate. 
            No synthetic vinegar, no artificial colors—only cold-pressed mustard oil, organic hand-picked spices, and authentic patience.
          </p>

          <!-- CTAs -->
          <div class="pt-2 flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4">
            <a href="#pickles" class="w-full sm:w-auto inline-flex items-center justify-center gap-3 bg-gradient-to-r from-brand-red to-brand-redhover text-white font-bold px-8 py-4 rounded-xl shadow-warm hover:shadow-xl hover:-translate-y-0.5 active:translate-y-0 transition duration-200">
              <i class="fa-solid fa-utensils text-sm text-brand-gold"></i>
              <span>Explore Pickles • अभी खरीदें</span>
            </a>
            
            <a href="tel:8383050500" class="w-full sm:w-auto inline-flex items-center justify-center gap-2.5 bg-white border border-brand-earth/15 hover:border-brand-green text-brand-greendark font-bold px-6 py-4 rounded-xl hover:bg-brand-creamlite shadow-sm transition duration-200">
              <i class="fa-solid fa-phone-volume text-brand-green"></i>
              <span>Call: 8383 0505 00</span>
            </a>
          </div>

          <!-- Trust Badges Row -->
          <div class="pt-6 border-t border-brand-earth/10 grid grid-cols-3 gap-4 max-w-lg mx-auto lg:mx-0 text-center sm:text-left">
            <div>
              <p class="font-serif text-2xl font-black text-brand-greendark">100%</p>
              <p class="text-xs font-medium text-brand-muted mt-0.5">Pure Mustard Oil</p>
            </div>
            <div>
              <p class="font-serif text-2xl font-black text-brand-greendark">0%</p>
              <p class="text-xs font-medium text-brand-muted mt-0.5">Chemicals & Preservatives</p>
            </div>
            <div>
              <p class="font-serif text-2xl font-black text-brand-greendark">FSSAI</p>
              <p class="text-xs font-medium text-brand-muted mt-0.5">Certified Kitchen</p>
            </div>
          </div>

        </div>

        <!-- Right Visual Showcase Banner -->
        <div class="lg:col-span-5 relative flex justify-center">
          <div class="relative w-full max-w-md">
            
            <!-- Glow background -->
            <div class="absolute -inset-4 bg-gradient-to-r from-brand-gold/40 to-brand-red/30 rounded-3xl blur-2xl opacity-60"></div>

            <!-- Featured Artisanal Card -->
            <div class="relative bg-white/90 backdrop-blur-md rounded-3xl p-6 sm:p-8 border border-brand-gold/30 shadow-2xl space-y-6">
              
              <div class="flex items-center justify-between pb-4 border-b border-brand-earth/10">
                <div class="flex items-center gap-2">
                  <span class="w-3 h-3 rounded-full bg-brand-red animate-pulse"></span>
                  <span class="text-xs uppercase font-extrabold tracking-wider text-brand-red">Authentic Barni Pickle</span>
                </div>
                <span class="text-xs font-bold px-2.5 py-1 rounded-full bg-brand-greenlight text-brand-green">450g Standard Jar</span>
              </div>

              <!-- Main Visual Representation -->
              <div class="relative h-64 sm:h-72 w-full rounded-2xl bg-gradient-to-b from-[#FFF2D6] to-[#FFE099] flex flex-col items-center justify-center overflow-hidden border border-amber-200">
                <div class="text-8xl sm:text-9xl filter drop-shadow-lg select-none hover:scale-110 transition duration-300">
                  🫙
                </div>
                <div class="absolute bottom-3 bg-brand-greendark/85 text-brand-gold px-4 py-1.5 rounded-full text-xs font-semibold backdrop-blur-sm">
                  सुगंधित राई & मेथी का तड़का
                </div>
              </div>

              <!-- Mini Pitch & Quick Add -->
              <div class="space-y-3">
                <div class="flex justify-between items-baseline">
                  <div>
                    <h3 class="font-serif font-black text-xl text-brand-greendark">Grandma's Heritage Mix</h3>
                    <p class="text-xs text-brand-muted font-hindi">परंपरागत स्वाद जो दिल छू ले</p>
                  </div>
                  <div class="text-right">
                    <span class="text-xs text-gray-400 line-through">₹299</span>
                    <span class="font-serif text-2xl font-black text-brand-red ml-1">₹249</span>
                  </div>
                </div>

                <button onclick="quickAddSample()" class="w-full bg-brand-green hover:bg-brand-greendark text-white font-bold py-3 rounded-xl flex items-center justify-center gap-2 shadow-md transition">
                  <i class="fa-solid fa-cart-plus text-brand-gold"></i>
                  <span>Quick Add to Bag</span>
                </button>
              </div>

            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- TRUST BADGES HIGHLIGHTS -->
  <section class="py-10 bg-white border-b border-brand-earth/10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-2 md:grid-cols-4 gap-6">
        
        <div class="flex items-center gap-3.5 p-3 rounded-xl bg-brand-cream/60 border border-brand-gold/20">
          <div class="w-12 h-12 rounded-xl bg-brand-gold/20 text-brand-golddark flex items-center justify-center text-xl shrink-0">
            <i class="fa-solid fa-seedling"></i>
          </div>
          <div>
            <h4 class="font-bold text-sm text-brand-greendark">100% Homemade</h4>
            <p class="text-xs text-brand-muted">Ghar ke masale se tayyar</p>
          </div>
        </div>

        <div class="flex items-center gap-3.5 p-3 rounded-xl bg-brand-cream/60 border border-brand-gold/20">
          <div class="w-12 h-12 rounded-xl bg-brand-greenlight text-brand-green flex items-center justify-center text-xl shrink-0">
            <i class="fa-solid fa-droplet"></i>
          </div>
          <div>
            <h4 class="font-bold text-sm text-brand-greendark">Cold-Pressed Mustard</h4>
            <p class="text-xs text-brand-muted">Pure Kachi Ghani Oil</p>
          </div>
        </div>

        <div class="flex items-center gap-3.5 p-3 rounded-xl bg-brand-cream/60 border border-brand-gold/20">
          <div class="w-12 h-12 rounded-xl bg-brand-red/15 text-brand-red flex items-center justify-center text-xl shrink-0">
            <i class="fa-solid fa-ban"></i>
          </div>
          <div>
            <h4 class="font-bold text-sm text-brand-greendark">Zero Chemicals</h4>
            <p class="text-xs text-brand-muted">No added artificial colors</p>
          </div>
        </div>

        <div class="flex items-center gap-3.5 p-3 rounded-xl bg-brand-cream/60 border border-brand-gold/20">
          <div class="w-12 h-12 rounded-xl bg-amber-100 text-amber-700 flex items-center justify-center text-xl shrink-0">
            <i class="fa-solid fa-sun"></i>
          </div>
          <div>
            <h4 class="font-bold text-sm text-brand-greendark">Sun-Cured Barnis</h4>
            <p class="text-xs text-brand-muted">Aged to supreme perfection</p>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- PRODUCT SHOWCASE SECTION -->
  <section id="pickles" class="py-16 md:py-24 relative">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      
      <!-- Section Header -->
      <div class="text-center max-w-3xl mx-auto mb-12 space-y-3">
        <span class="text-xs md:text-sm uppercase tracking-widest font-extrabold text-brand-red font-hindi">हाथों से तैयार पारंपरिक स्वाद</span>
        <h2 class="font-serif text-3xl sm:text-4xl md:text-5xl font-black text-brand-greendark">
          Our Signature Pickle Collection
        </h2>
        <p class="text-sm md:text-base text-brand-muted">
          Every jar is made in small artisanal batches of 450 grams using farm-fresh vegetables and slow-cooked sun infusion.
        </p>
      </div>

      <!-- Live Interactive Products Grid (Populated dynamically) -->
      <div id="productGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6 sm:gap-8">
        <!-- Rendered via JS -->
        <div class="col-span-full py-20 text-center">
          <div class="inline-block animate-spin text-brand-gold text-4xl mb-4"><i class="fa-solid fa-circle-notch"></i></div>
          <p class="text-brand-muted font-medium">अचारों की सूची लोड हो रही है (Loading delicious pickles)...</p>
        </div>
      </div>

    </div>
  </section>

  <!-- WHY MINDO HERITAGE PROCESS -->
  <section id="why-us" class="py-16 md:py-24 bg-gradient-to-b from-white to-[#FAF4E6] border-y border-brand-earth/10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      
      <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
        <span class="text-xs uppercase font-bold tracking-widest text-brand-golddark">Pure Tradition</span>
        <h2 class="font-serif text-3xl sm:text-4xl font-black text-brand-greendark">Mindo का अचार क्यों है खास?</h2>
        <p class="text-brand-muted text-sm sm:text-base">जब बात सेहत और स्वाद की हो, तो घर जैसा कोई विकल्प नहीं।</p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
        
        <!-- Step 1 -->
        <div class="bg-white p-6 rounded-2xl border border-brand-gold/30 shadow-sm hover:shadow-md transition text-center space-y-4">
          <div class="w-16 h-16 mx-auto rounded-2xl bg-amber-50 text-brand-golddark flex items-center justify-center text-3xl">
            🫙
          </div>
          <h3 class="font-serif font-black text-lg text-brand-greendark">1. शुध्द कच्ची घानी सरसों</h3>
          <p class="text-xs sm:text-sm text-brand-muted leading-relaxed">
            हर अचार सिर्फ और सिर्फ प्रीमियम सरसों तेल में बनाया जाता है ताकि असली पंजेंट और नेचुरल फ्लेवर मिले।
          </p>
        </div>

        <!-- Step 2 -->
        <div class="bg-white p-6 rounded-2xl border border-brand-gold/30 shadow-sm hover:shadow-md transition text-center space-y-4">
          <div class="w-16 h-16 mx-auto rounded-2xl bg-red-50 text-brand-red flex items-center justify-center text-3xl">
            🌶️
          </div>
          <h3 class="font-serif font-black text-lg text-brand-greendark">2. साबुत कुटे हुए मसाले</h3>
          <p class="text-xs sm:text-sm text-brand-muted leading-relaxed">
            राई, सौंफ, मेथीदाना, अजवाइन और हींग—हर मसाला धीमी आंच पर भूनकर दरदरा कूटा जाता है।
          </p>
        </div>

        <!-- Step 3 -->
        <div class="bg-white p-6 rounded-2xl border border-brand-gold/30 shadow-sm hover:shadow-md transition text-center space-y-4">
          <div class="w-16 h-16 mx-auto rounded-2xl bg-emerald-50 text-brand-green flex items-center justify-center text-3xl">
            🧼
          </div>
          <h3 class="font-serif font-black text-lg text-brand-greendark">3. हाइजीन और प्यार</h3>
          <p class="text-xs sm:text-sm text-brand-muted leading-relaxed">
            FSSAI सर्टिफाइड मानकों के अनुसार साफ़-सफ़ाई के साथ पारंपरिक मिट्टी और चीनी मिट्टी की बरनियों में संरक्षित।
          </p>
        </div>

        <!-- Step 4 -->
        <div class="bg-white p-6 rounded-2xl border border-brand-gold/30 shadow-sm hover:shadow-md transition text-center space-y-4">
          <div class="w-16 h-16 mx-auto rounded-2xl bg-amber-50 text-amber-600 flex items-center justify-center text-3xl">
            ☀️
          </div>
          <h3 class="font-serif font-black text-lg text-brand-greendark">4. प्राकृतिक धूप में पकाई</h3>
          <p class="text-xs sm:text-sm text-brand-muted leading-relaxed">
            बिना किसी केमिकल एसिड के, छतों पर धूप की किरणों में हफ्तों तक प्राकृतिक रूप से तैयार।
          </p>
        </div>

      </div>

    </div>
  </section>

  <!-- SPICE INGREDIENTS BANNER -->
  <section id="ingredients" class="py-14 bg-gradient-to-r from-brand-greendark to-brand-green text-white relative overflow-hidden">
    <div class="max-w-6xl mx-auto px-4 text-center space-y-4 relative z-10">
      <div class="inline-flex items-center gap-2 bg-white/10 px-4 py-1.5 rounded-full text-xs font-semibold text-brand-gold">
        <i class="fa-solid fa-mortar-pestle"></i> 100% Natural Farm Sourced
      </div>
      <h2 class="font-serif text-3xl sm:text-4xl font-black text-brand-gold">पवित्र मसालों का संगम</h2>
      <p class="text-sm sm:text-base text-gray-200 max-w-3xl mx-auto leading-relaxed">
        Green Chilli, Iodised Salt, Mustard Oil, Red Chilli, Cumin, Saunf, Ajwain, Turmeric, Hing (Asafoetida), Black Pepper, Mustard Seeds & Handpicked Indigenous Condiments.
      </p>
      <div class="pt-4 flex flex-wrap justify-center gap-2 text-xs font-semibold">
        <span class="bg-white/10 px-3 py-1.5 rounded-full">🌱 No Artificial Vinegar</span>
        <span class="bg-white/10 px-3 py-1.5 rounded-full">🌿 Zero Food Coloring</span>
        <span class="bg-white/10 px-3 py-1.5 rounded-full">🫙 Traditional Ceramic Cure</span>
      </div>
    </div>
  </section>

  <!-- TESTIMONIALS / CUSTOMER EXPERIENCES -->
  <section id="reviews" class="py-16 md:py-24">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      
      <div class="text-center max-w-2xl mx-auto mb-14 space-y-2">
        <span class="text-xs uppercase font-extrabold tracking-widest text-brand-red">Real Verified Reviews</span>
        <h2 class="font-serif text-3xl sm:text-4xl font-black text-brand-greendark">हमारे ग्राहकों की राय</h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 sm:gap-8">
        
        <div class="bg-white p-7 rounded-2xl border border-brand-earth/10 shadow-sm hover:shadow-warm transition space-y-4">
          <div class="flex text-amber-400 text-sm gap-1">
            <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>
          </div>
          <p class="text-sm text-brand-earth/80 italic leading-relaxed">
            "बिल्कुल घर जैसा स्वाद! लाल मिर्च का भरवा अचार तो कमाल का है – माँ के हाथ का अचार याद आ गया। तेल बिल्कुल हल्का और असली है।"
          </p>
          <div class="flex items-center gap-3 pt-2 border-t border-gray-100">
            <div class="w-10 h-10 rounded-full bg-brand-green/20 text-brand-green font-bold flex items-center justify-center text-sm">
              RS
            </div>
            <div>
              <h4 class="font-bold text-sm text-brand-greendark">Rohit Sharma</h4>
              <p class="text-xs text-brand-muted">Delhi • Verified Buyer</p>
            </div>
          </div>
        </div>

        <div class="bg-white p-7 rounded-2xl border border-brand-earth/10 shadow-sm hover:shadow-warm transition space-y-4">
          <div class="flex text-amber-400 text-sm gap-1">
            <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>
          </div>
          <p class="text-sm text-brand-earth/80 italic leading-relaxed">
            "मिक्स अचार में असली मसालों का स्वाद है, बाजार वाले केमिकल पिकल जैसे गले में नहीं लगता। पराठों के साथ रोज़ खाते हैं!"
          </p>
          <div class="flex items-center gap-3 pt-2 border-t border-gray-100">
            <div class="w-10 h-10 rounded-full bg-brand-gold/20 text-brand-golddark font-bold flex items-center justify-center text-sm">
              PV
            </div>
            <div>
              <h4 class="font-bold text-sm text-brand-greendark">Priya Verma</h4>
              <p class="text-xs text-brand-muted">Noida • Regular Customer</p>
            </div>
          </div>
        </div>

        <div class="bg-white p-7 rounded-2xl border border-brand-earth/10 shadow-sm hover:shadow-warm transition space-y-4">
          <div class="flex text-amber-400 text-sm gap-1">
            <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>
          </div>
          <p class="text-sm text-brand-earth/80 italic leading-relaxed">
            "शुद्ध सरसों तेल की खुशबू ढक्कन खोलते ही आ जाती है। डिलीवरी भी बहुत फ़ास्ट हुई और पैकिंग बहुत सेफ थी।"
          </p>
          <div class="flex items-center gap-3 pt-2 border-t border-gray-100">
            <div class="w-10 h-10 rounded-full bg-brand-red/20 text-brand-red font-bold flex items-center justify-center text-sm">
              AK
            </div>
            <div>
              <h4 class="font-bold text-sm text-brand-greendark">Amit Kumar</h4>
              <p class="text-xs text-brand-muted">Gurugram • Foodie</p>
            </div>
          </div>
        </div>

      </div>

    </div>
  </section>

  <!-- CONTACT & ORDER FOOTPRINT -->
  <section id="contact" class="py-16 bg-white border-t border-brand-earth/10">
    <div class="max-w-5xl mx-auto px-4 sm:px-6">
      
      <div class="bg-gradient-to-br from-brand-cream to-white rounded-3xl p-8 sm:p-12 border border-brand-gold/40 shadow-xl text-center space-y-6">
        
        <span class="inline-block px-4 py-1 rounded-full bg-brand-greenlight text-brand-green font-bold text-xs uppercase tracking-wider">
          Direct Kitchen Connect
        </span>

        <h2 class="font-serif text-3xl sm:text-4xl font-black text-brand-greendark">
          ऑर्डर या किसी भी प्रश्न के लिए संपर्क करें
        </h2>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 pt-4 text-left">
          
          <div class="p-4 rounded-xl bg-white border border-gray-200">
            <p class="text-xs font-semibold text-brand-muted">📞 Direct Support / Order</p>
            <a href="tel:8383050500" class="text-base font-extrabold text-brand-greendark hover:text-brand-red transition block mt-1">
              8383 0505 00
            </a>
          </div>

          <div class="p-4 rounded-xl bg-white border border-gray-200">
            <p class="text-xs font-semibold text-brand-muted">✉️ Email Inquiry</p>
            <a href="mailto:sanatan.ent500@gmail.com" class="text-sm font-bold text-brand-greendark hover:text-brand-red transition block mt-1 break-words">
              sanatan.ent500@gmail.com
            </a>
          </div>

          <div class="p-4 rounded-xl bg-white border border-gray-200">
            <p class="text-xs font-semibold text-brand-muted">📍 Registered Facility</p>
            <p class="text-xs font-medium text-brand-earth mt-1 leading-snug">
              Sanatan Enterprises, F Block, School Road, Khanpur, South Delhi – 110062
            </p>
          </div>

        </div>

        <div class="pt-4 flex flex-wrap justify-center gap-4">
          <a href="https://wa.me/918383050500?text=Namaste%20Mindo!%20I%20want%20to%20order%20pickles" target="_blank" class="bg-emerald-600 hover:bg-emerald-700 text-white font-bold px-7 py-3 rounded-xl inline-flex items-center gap-2 shadow-md hover:shadow-lg transition">
            <i class="fa-brands fa-whatsapp text-lg"></i>
            <span>WhatsApp पर ऑर्डर करें</span>
          </a>

          <a href="tel:8383050500" class="bg-brand-greendark hover:bg-brand-green text-white font-bold px-7 py-3 rounded-xl inline-flex items-center gap-2 shadow-md transition">
            <i class="fa-solid fa-phone text-sm text-brand-gold"></i>
            <span>Call Now</span>
          </a>
        </div>

        <div class="pt-4">
          <span class="inline-flex items-center gap-2 bg-[#EAF5ED] text-brand-green text-xs font-semibold px-4 py-2 rounded-full border border-emerald-200">
            <i class="fa-solid fa-shield-halved"></i> FSSAI Lic. No.: 23325002004226
          </span>
        </div>

      </div>

    </div>
  </section>

  <!-- FOOTER -->
  <footer class="bg-brand-earth text-brand-cream/80 pt-12 pb-8 border-t border-white/10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center space-y-4">
      <div class="font-serif font-black text-2xl text-brand-gold">Mindo Pickles</div>
      <p class="text-xs max-w-md mx-auto text-brand-cream/60">
        शुद्धता, स्वास्थ्य और प्राचीन भारतीय स्वाद का प्रतीक। दादी-नानी के पारंपरिक नुस्खों से प्रेरित।
      </p>
      <div class="text-xs text-brand-cream/40 pt-4 border-t border-white/10">
        © <span id="yr"></span> Mindo – Manufactured & Marketed by Sanatan Enterprises. All rights reserved.
      </div>
    </div>
  </footer>

  <!-- FLOATING ACTION BUTTONS -->
  
  <!-- WhatsApp Floating Trigger -->
  <a href="https://wa.me/918383050500?text=Namaste%20Mindo!%20I%20want%20to%20order%20fresh%20pickles" target="_blank" class="fixed right-5 bottom-6 z-40 bg-emerald-600 hover:bg-emerald-700 text-white w-14 h-14 rounded-full flex items-center justify-center text-2xl shadow-floating hover:scale-110 transition-all duration-300">
    <i class="fa-brands fa-whatsapp"></i>
  </a>

  <!-- Cart Floating Sticky Trigger -->
  <button onclick="openCart()" class="fixed right-5 bottom-24 z-40 bg-brand-gold hover:bg-brand-golddark text-brand-earth w-14 h-14 rounded-full flex items-center justify-center text-xl shadow-floating hover:scale-110 transition-all duration-300">
    <i class="fa-solid fa-basket-shopping text-brand-earth"></i>
    <span id="floatCartBadge" class="absolute -top-1 -right-1 bg-brand-red text-white text-[11px] font-black h-5 w-5 rounded-full flex items-center justify-center border-2 border-white">0</span>
  </button>

  <!-- Hidden Discreet Admin Trigger Button -->
  <button onclick="openAdmin()" title="Admin Control" class="fixed left-4 bottom-4 z-40 w-8 h-8 rounded-full bg-brand-earth/20 hover:bg-brand-green text-brand-earth/60 hover:text-white flex items-center justify-center text-xs backdrop-blur-sm transition duration-300">
    <i class="fa-solid fa-gear"></i>
  </button>

  <!-- ============================================================
       MODAL 1: LUXURY CART & CHECKOUT DRAWER
  ============================================================ -->
  <div id="cartModal" class="fixed inset-0 z-50 bg-black/60 backdrop-blur-sm hidden items-center justify-center p-3 sm:p-4 overflow-y-auto">
    <div class="relative bg-white rounded-3xl max-w-lg w-full p-6 sm:p-8 shadow-2xl border border-brand-gold/30 animate-in fade-in zoom-in duration-200 my-auto">
      
      <!-- Close Button -->
      <button onclick="closeModal('cartModal')" class="absolute top-5 right-5 text-gray-400 hover:text-brand-red text-xl w-8 h-8 rounded-full bg-gray-100 flex items-center justify-center transition">
        <i class="fa-solid fa-xmark"></i>
      </button>

      <!-- Cart Dynamic Injected Body -->
      <div id="cartContent">
        <!-- Rendered by renderCartContent() -->
      </div>

    </div>
  </div>

  <!-- ============================================================
       MODAL 2: ADMIN PANEL (LOGIN & DASHBOARD)
  ============================================================ -->
  <div id="adminModal" class="fixed inset-0 z-50 bg-black/65 backdrop-blur-md hidden items-center justify-center p-3 sm:p-6 overflow-y-auto">
    <div class="relative bg-white rounded-3xl max-w-3xl w-full p-6 sm:p-8 shadow-2xl border border-brand-earth/20 my-auto">
      
      <!-- Close Button -->
      <button onclick="closeModal('adminModal')" class="absolute top-5 right-5 text-gray-400 hover:text-brand-red text-xl w-8 h-8 rounded-full bg-gray-100 flex items-center justify-center transition">
        <i class="fa-solid fa-xmark"></i>
      </button>

      <div id="adminContent">
        <!-- Injected via renderAdminLogin() or renderAdminDashboard() -->
      </div>

    </div>
  </div>

  <!-- TOAST NOTIFICATIONS -->
  <div id="toast" class="fixed bottom-8 left-1/2 -translate-x-1/2 z-50 bg-brand-earth text-white px-6 py-3 rounded-full font-semibold text-sm shadow-2xl pointer-events-none opacity-0 -translate-y-4 transition-all duration-300 flex items-center gap-2">
    <span>Notification</span>
  </div>

  <!-- ============================================================
       FIREBASE SCRIPTS (Compat v9 for existing DB schema)
  ============================================================ -->
  <script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-app-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-database-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-auth-compat.js"></script>

  <script>
    /* ============================================================
       FIREBASE CONFIG & ESSENTIALS
    ============================================================ */
    const firebaseConfig = {
      apiKey: "AIzaSyAKe_cHTWNYerJCo6drMPn2wOi59HJR8XQ",
      authDomain: "kapilmindo-3c257.firebaseapp.com",
      databaseURL: "https://kapilmindo-3c257-default-rtdb.firebaseio.com",
      projectId: "kapilmindo-3c257",
      storageBucket: "kapilmindo-3c257.firebasestorage.app",
      messagingSenderId: "280067203318",
      appId: "1:280067203318:web:98bd3da14eee3a2f900cd7",
      measurementId: "G-CHRK14YN6D"
    };

    const IMG_BASE = "./";
    const PHONE = "918383050500";

    // Application State
    let db = null;
    let auth = null;
    let firebaseReady = false;
    let products = [];
    let cart = [];
    let paymentSettings = { qrCode: "", upiId: "8383050500@ybl" };
    let isAdmin = false;
    let adminTab = "orders";
    let showAllProducts = false;

    // Default Fallback Pickles Catalog if empty
    const DEFAULT_PRODUCTS = [
      {
        id: "p_mango",
        name: "Heritage Aam Ka Achar",
        hi: "पारंपरिक आम का अचार",
        tag: "कच्ची कैरी, सौंफ, मेथी और शुद्ध सरसों तेल का बेजोड़ स्वाद।",
        price: 249,
        mrp: 299,
        emoji: "🥭",
        img: "",
        bestseller: true
      },
      {
        id: "p_redchilli",
        name: "Banarasi Bharwa Lal Mirch",
        hi: "बनारसी भरवा लाल मिर्च",
        tag: "मोटी लाल मिर्च में भरा हाथ से पिसा अमचूर व राई का मसाला।",
        price: 279,
        mrp: 320,
        emoji: "🌶️",
        img: "",
        bestseller: true
      },
      {
        id: "p_lemon",
        name: "Khatta Meetha Nimbu",
        hi: "खट्टा मीठा नींबू अचार",
        tag: "धूप में पका पतला छिलका नींबू, अजवाइन और हींग युक्त पाचनवर्धक।",
        price: 220,
        mrp: 260,
        emoji: "🍋",
        img: "",
        bestseller: false
      },
      {
        id: "p_greenchilli",
        name: "Hari Mirch Rahi Ka Tadka",
        hi: "तीखी हरी मिर्च का अचार",
        tag: "कुरकुरी हरी मिर्च, पीली सरसों व कलौंजी के साथ तीखा स्वाद।",
        price: 210,
        mrp: 250,
        emoji: "🌿",
        img: "",
        bestseller: false
      },
      {
        id: "p_mixed",
        name: "Pachranga Mix Special",
        hi: "स्पेशल पंचरंगा मिक्स अचार",
        tag: "गाजर, गोभी, शलगम और कैरी का समृद्ध पारिवारिक संगम।",
        price: 249,
        mrp: 299,
        emoji: "🫙",
        img: "",
        bestseller: true
      }
    ];

    /* ============================================================
       INITIALIZATION
    ============================================================ */
    async function init() {
      // Safe cart recovery
      try {
        const savedCart = localStorage.getItem("mindo_cart");
        if (savedCart) cart = JSON.parse(savedCart);
      } catch (e) {
        cart = [];
      }

      // Initialize Firebase
      try {
        if (typeof firebase !== 'undefined' && firebaseConfig.apiKey) {
          firebase.initializeApp(firebaseConfig);
          db = firebase.database();
          auth = firebase.auth();
          firebaseReady = true;

          auth.onAuthStateChanged(user => {
            isAdmin = !!user;
            if (document.getElementById("adminModal").classList.contains("flex")) {
              if (isAdmin) renderAdminDashboard();
              else renderAdminLogin();
            }
          });
        }
      } catch (err) {
        console.warn("Firebase Init note: Local store will be active.", err);
      }

      await loadProducts();
      await loadPaymentSettings();
      renderProducts();
      updateCartBadge();
      
      const yrEl = document.getElementById("yr");
      if (yrEl) yrEl.textContent = new Date().getFullYear();
    }

    /* ============================================================
       PRODUCTS MANAGEMENT
    ============================================================ */
    async function loadProducts() {
      if (firebaseReady) {
        try {
          const snapshot = await db.ref('products').once('value');
          const data = snapshot.val();
          if (data) {
            products = Object.keys(data).map(key => ({ id: key, ...data[key] }));
          } else {
            // Seed defaults if fresh DB
            products = [...DEFAULT_PRODUCTS];
          }
        } catch (e) {
          console.error("Products load error:", e);
          loadLocalProducts();
        }
      } else {
        loadLocalProducts();
      }
    }

    function loadLocalProducts() {
      const cached = localStorage.getItem("mindo_products_new");
      products = cached ? JSON.parse(cached) : [...DEFAULT_PRODUCTS];
    }

    function renderProducts() {
      const grid = document.getElementById("productGrid");
      if (!grid) return;

      if (!products.length) {
        grid.innerHTML = `
          <div class="col-span-full py-12 text-center bg-white rounded-3xl border border-brand-earth/10">
            <span class="text-5xl block mb-2">🫙</span>
            <p class="font-bold text-brand-greendark text-lg">अभी कोई प्रोडक्ट उपलब्ध नहीं है</p>
            <p class="text-sm text-brand-muted">एडमिन पैनल से नए अचार जोड़ें।</p>
          </div>
        `;
        return;
      }

      const displayProducts = showAllProducts ? products : products.slice(0, 8);

      let html = displayProducts.map((p, idx) => {
        const imgUrl = p.img ? (p.img.startsWith("http") || p.img.startsWith("data:") ? p.img : IMG_BASE + p.img) : "";
        
        return `
          <div class="group bg-white rounded-3xl p-5 border border-brand-gold/30 shadow-sm hover:shadow-card-hover transition-all duration-300 flex flex-col justify-between relative overflow-hidden">
            
            ${p.bestseller ? `
              <div class="absolute top-4 left-4 z-10 bg-brand-red text-white text-[11px] font-extrabold px-3 py-1 rounded-full uppercase tracking-wider shadow-sm flex items-center gap-1">
                <i class="fa-solid fa-star text-[10px] text-brand-gold"></i> Bestseller
              </div>
            ` : ''}

            <!-- Jar Visual / Image Area -->
            <div class="relative h-56 rounded-2xl bg-gradient-to-tr from-[#FFF3DA] to-[#FFE5AF] flex items-center justify-center overflow-hidden mb-4 group-hover:scale-[1.02] transition-transform duration-300">
              ${imgUrl ? `
                <img src="${imgUrl}" alt="${p.name}" class="w-full h-full object-cover">
              ` : `
                <span class="text-7xl filter drop-shadow select-none group-hover:rotate-6 transition-transform duration-300">${p.emoji || "🫙"}</span>
              `}
              <div class="absolute bottom-2.5 right-2.5 bg-brand-greendark/90 text-brand-gold text-[11px] font-bold px-2.5 py-1 rounded-full backdrop-blur-sm">
                450g Jar
              </div>
            </div>

            <!-- Body Details -->
            <div class="space-y-2 flex-1 flex flex-col justify-between">
              <div>
                <h3 class="font-serif font-black text-lg text-brand-greendark group-hover:text-brand-red transition-colors leading-snug">
                  ${p.name}
                </h3>
                ${p.hi ? `<p class="font-hindi text-xs text-brand-red font-semibold">${p.hi}</p>` : ''}
                <p class="text-xs text-brand-muted line-clamp-2 mt-1.5 leading-relaxed">${p.tag || "शुद्ध सरसों तेल और दादी-नानी के पारंपरिक मसाले से निर्मित।"}</p>
              </div>

              <!-- Price & Add Action -->
              <div class="pt-4 mt-2 border-t border-brand-earth/10 flex items-center justify-between">
                <div>
                  <span class="text-xs text-gray-400 line-through">${p.mrp ? `₹${p.mrp}` : ''}</span>
                  <div class="font-serif font-black text-2xl text-brand-red leading-none">
                    ₹${p.price}
                  </div>
                </div>

                <button onclick="addToCartByIndex(${idx})" class="bg-brand-green hover:bg-brand-greendark text-white font-bold px-4 py-2.5 rounded-xl text-xs flex items-center gap-2 shadow-sm hover:shadow transition-all active:scale-95">
                  <i class="fa-solid fa-cart-shopping text-brand-gold"></i>
                  <span>Add to Bag</span>
                </button>
              </div>

            </div>

          </div>
        `;
      }).join("");

      if (!showAllProducts && products.length > 8) {
        html += `
          <div onclick="showAllPickles()" class="bg-brand-cream/80 hover:bg-amber-100/70 border-2 border-dashed border-brand-gold/60 rounded-3xl p-6 flex flex-col items-center justify-center text-center cursor-pointer transition group min-h-[360px]">
            <div class="w-16 h-16 rounded-full bg-brand-gold/20 text-brand-green flex items-center justify-center text-3xl mb-4 group-hover:scale-110 transition">
              <i class="fa-solid fa-plus"></i>
            </div>
            <h3 class="font-serif font-black text-xl text-brand-greendark mb-1">See All Pickles</h3>
            <p class="text-xs text-brand-muted font-hindi">सभी ${products.length} पारंपरिक अचार देखें</p>
          </div>
        `;
      }

      grid.innerHTML = html;
    }

    function showAllPickles() {
      showAllProducts = true;
      renderProducts();
    }

    function quickAddSample() {
      if (products.length > 0) {
        addToCart(products[0]);
      } else {
        addToCart({ name: "Mindo Heritage Mix Jar", price: 249, emoji: "🫙" });
      }
    }

    function addToCartByIndex(index) {
      if (products[index]) addToCart(products[index]);
    }

    /* ============================================================
       CART LOGIC & REALTIME STATE
    ============================================================ */
    function addToCart(item) {
      const existing = cart.find(i => i.name === item.name);
      if (existing) {
        existing.qty += 1;
      } else {
        cart.push({
          name: item.name,
          price: Number(item.price),
          emoji: item.emoji || "🫙",
          img: item.img || "",
          qty: 1
        });
      }
      saveCart();
      updateCartBadge();
      toast("✅ कार्ट में जोड़ा गया! (" + item.name + ")", "success");
    }

    function saveCart() {
      localStorage.setItem("mindo_cart", JSON.stringify(cart));
    }

    function updateCartBadge() {
      const count = cart.reduce((sum, item) => sum + item.qty, 0);
      const navBadge = document.getElementById("navCartBadge");
      const floatBadge = document.getElementById("floatCartBadge");
      
      if (navBadge) navBadge.textContent = count;
      if (floatBadge) floatBadge.textContent = count;
    }

    function updateQty(index, delta) {
      if (!cart[index]) return;
      cart[index].qty += delta;
      if (cart[index].qty <= 0) {
        cart.splice(index, 1);
      }
      saveCart();
      updateCartBadge();
      renderCartContent();
    }

    function removeFromCart(index) {
      if (!cart[index]) return;
      cart.splice(index, 1);
      saveCart();
      updateCartBadge();
      renderCartContent();
    }

    function openCart() {
      const modal = document.getElementById("cartModal");
      modal.classList.remove("hidden");
      modal.classList.add("flex");
      document.body.style.overflow = "hidden";
      renderCartContent();
    }

    function renderCartContent() {
      const container = document.getElementById("cartContent");
      if (!container) return;

      if (!cart.length) {
        container.innerHTML = `
          <div class="text-center py-12 space-y-4">
            <div class="w-20 h-20 mx-auto rounded-full bg-brand-cream text-brand-golddark flex items-center justify-center text-4xl">
              <i class="fa-solid fa-basket-shopping"></i>
            </div>
            <h3 class="font-serif font-black text-2xl text-brand-greendark">आपका कार्ट अभी खाली है</h3>
            <p class="text-xs sm:text-sm text-brand-muted max-w-xs mx-auto">स्वादिष्ट और शुद्ध देसी अचार चुनें और अपने भोजन का स्वाद बढ़ाएं।</p>
            <button onclick="closeModal('cartModal')" class="bg-brand-green text-white font-bold px-6 py-2.5 rounded-xl text-sm shadow hover:bg-brand-greendark transition">
              Explore Pickles
            </button>
          </div>
        `;
        return;
      }

      const total = cart.reduce((sum, item) => sum + (item.price * item.qty), 0);

      const itemsHtml = cart.map((item, idx) => {
        const imgUrl = item.img ? (item.img.startsWith("http") || item.img.startsWith("data:") ? item.img : IMG_BASE + item.img) : "";
        return `
          <div class="flex items-center justify-between gap-3 py-3 border-b border-gray-100">
            <div class="flex items-center gap-3">
              <div class="w-12 h-12 rounded-xl bg-amber-50 flex items-center justify-center overflow-hidden shrink-0 border border-amber-200">
                ${imgUrl ? `<img src="${imgUrl}" class="w-full h-full object-cover">` : `<span class="text-2xl">${item.emoji || "🫙"}</span>`}
              </div>
              <div>
                <h4 class="font-bold text-xs sm:text-sm text-brand-greendark">${item.name}</h4>
                <p class="text-xs font-serif font-bold text-brand-red">₹${item.price} each</p>
              </div>
            </div>

            <!-- Qty controller -->
            <div class="flex items-center gap-3">
              <div class="flex items-center bg-gray-100 rounded-lg p-1 border border-gray-200">
                <button onclick="updateQty(${idx}, -1)" class="w-6 h-6 flex items-center justify-center text-gray-700 font-bold hover:text-brand-red">−</button>
                <span class="w-7 text-center font-bold text-xs">${item.qty}</span>
                <button onclick="updateQty(${idx}, 1)" class="w-6 h-6 flex items-center justify-center text-gray-700 font-bold hover:text-brand-green">+</button>
              </div>
              <button onclick="removeFromCart(${idx})" class="text-gray-400 hover:text-brand-red text-sm transition">
                <i class="fa-regular fa-trash-can"></i>
              </button>
            </div>
          </div>
        `;
      }).join("");

      // Dynamic QR Code generation for seamless direct UPI payment
      const upiString = `upi://pay?pa=${paymentSettings.upiId || '8383050500@ybl'}&pn=MindoPickles&am=${total}&cu=INR`;
      const qrCodeApiUrl = paymentSettings.qrCode 
        ? paymentSettings.qrCode 
        : `https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=${encodeURIComponent(upiString)}`;

      container.innerHTML = `
        <div class="space-y-4">
          <div class="flex items-center justify-between pb-3 border-b border-gray-100">
            <h3 class="font-serif font-black text-2xl text-brand-greendark flex items-center gap-2">
              <i class="fa-solid fa-basket-shopping text-brand-gold"></i> Your Order
            </h3>
            <span class="text-xs font-bold text-brand-muted">${cart.length} item(s)</span>
          </div>

          <!-- Items Scroll Area -->
          <div class="max-h-56 overflow-y-auto pr-1">
            ${itemsHtml}
          </div>

          <!-- Total Calculation Pill -->
          <div class="bg-brand-cream/90 p-4 rounded-2xl flex items-center justify-between border border-brand-gold/30">
            <div>
              <p class="text-xs text-brand-muted font-semibold">Total Payable Amount</p>
              <p class="text-[11px] text-brand-green font-bold">Free Shipping on Prepaid / WhatsApp Confirmation</p>
            </div>
            <div class="font-serif font-black text-3xl text-brand-red">₹${total}</div>
          </div>

          <!-- Checkout Details Form -->
          <form onsubmit="submitCartOrder(event)" class="space-y-3 pt-2">
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
              <div>
                <label class="block text-xs font-bold text-brand-earth mb-1">आपका नाम (Full Name) *</label>
                <input type="text" name="customerName" required placeholder="जैसे: Rajesh Sharma" class="w-full text-xs sm:text-sm px-3.5 py-2.5 rounded-xl border border-gray-300 focus:border-brand-green focus:ring-1 focus:ring-brand-green outline-none">
              </div>
              <div>
                <label class="block text-xs font-bold text-brand-earth mb-1">मोबाइल नंबर (Phone) *</label>
                <input type="tel" name="phone" required placeholder="10-digit WhatsApp No." class="w-full text-xs sm:text-sm px-3.5 py-2.5 rounded-xl border border-gray-300 focus:border-brand-green focus:ring-1 focus:ring-brand-green outline-none">
              </div>
            </div>

            <div>
              <label class="block text-xs font-bold text-brand-earth mb-1">पूरा डिलीवरी पता (Complete Delivery Address) *</label>
              <textarea name="address" required rows="2" placeholder="House/Flat No, Street, Landmark, City, State, PIN Code" class="w-full text-xs sm:text-sm px-3.5 py-2 rounded-xl border border-gray-300 focus:border-brand-green focus:ring-1 focus:ring-brand-green outline-none"></textarea>
            </div>

            <div>
              <label class="block text-xs font-bold text-brand-earth mb-1">कोई स्पेशल नोट (Special Instruction - Optional)</label>
              <input type="text" name="note" placeholder="जैसे: कम तीखा या अतिरिक्त पैकिंग" class="w-full text-xs sm:text-sm px-3.5 py-2 rounded-xl border border-gray-300 focus:border-brand-green focus:ring-1 focus:ring-brand-green outline-none">
            </div>

            <!-- Instant UPI Scan Section -->
            <div class="p-4 rounded-2xl bg-amber-50/70 border border-amber-200 text-center space-y-2">
              <p class="text-xs font-bold text-brand-greendark flex items-center justify-center gap-1.5">
                <i class="fa-solid fa-qrcode text-brand-golddark"></i> Scan & Pay via any UPI App (GPay, PhonePe, Paytm)
              </p>
              
              <div class="inline-block p-2 bg-white rounded-xl shadow-sm border border-amber-300">
                <img src="${qrCodeApiUrl}" alt="UPI QR Code" class="w-32 h-32 mx-auto object-contain">
              </div>

              <div class="text-[11px] font-mono font-semibold text-brand-earth bg-white/80 py-1 px-3 rounded-lg inline-block border border-gray-200">
                UPI ID: ${paymentSettings.upiId || '8383050500@ybl'}
              </div>
            </div>

            <!-- Submit Button -->
            <button type="submit" id="submitCartBtn" class="w-full bg-gradient-to-r from-brand-green to-brand-greendark hover:from-brand-greendark hover:to-brand-green text-white font-extrabold py-3.5 rounded-xl shadow-warm flex items-center justify-center gap-2 text-sm transition">
              <i class="fa-brands fa-whatsapp text-lg text-emerald-400"></i>
              <span>ऑर्डर कन्फर्म करें (Place Order ₹${total})</span>
            </button>
          </form>
        </div>
      `;
    }

    async function submitCartOrder(e) {
      e.preventDefault();
      const btn = document.getElementById("submitCartBtn");
      btn.disabled = true;
      btn.innerHTML = `<i class="fa-solid fa-spinner animate-spin"></i> Placing Order...`;

      const fd = new FormData(e.target);
      const total = cart.reduce((sum, item) => sum + (item.price * item.qty), 0);

      const orderData = {
        customerName: fd.get("customerName").trim(),
        phone: fd.get("phone").trim(),
        address: fd.get("address").trim(),
        note: fd.get("note").trim(),
        items: cart.map(item => ({
          name: item.name,
          price: item.price,
          qty: item.qty,
          emoji: item.emoji || "🫙"
        })),
        total,
        status: "pending"
      };

      try {
        let orderId;
        if (firebaseReady) {
          const ref = db.ref('orders').push();
          await ref.set({
            ...orderData,
            createdAt: firebase.database.ServerValue.TIMESTAMP
          });
          orderId = ref.key.slice(-6).toUpperCase();
        } else {
          orderId = "MND" + Date.now().toString().slice(-5);
          const orders = JSON.parse(localStorage.getItem("mindo_orders") || "[]");
          orders.push({ id: orderId, ...orderData, createdAt: Date.now() });
          localStorage.setItem("mindo_orders", JSON.stringify(orders));
        }

        const itemsString = cart.map(item => `${item.name} (${item.qty} jar)`).join(", ");
        const waMsg = encodeURIComponent(
          `Namaste Mindo Pickles! I have placed an order.\n\n` +
          `Order ID: #${orderId}\n` +
          `Name: ${orderData.customerName}\n` +
          `Phone: ${orderData.phone}\n` +
          `Items: ${itemsString}\n` +
          `Total: ₹${total}\n` +
          `Address: ${orderData.address}\n` +
          `${orderData.note ? `Note: ${orderData.note}\n` : ''}` +
          `\nPlease confirm my dispatch!`
        );

        // Success Confirmation View
        document.getElementById("cartContent").innerHTML = `
          <div class="text-center py-6 space-y-4">
            <div class="w-16 h-16 mx-auto rounded-full bg-emerald-100 text-emerald-600 flex items-center justify-center text-3xl">
              <i class="fa-solid fa-circle-check"></i>
            </div>
            <h3 class="font-serif font-black text-2xl text-brand-greendark">ऑर्डर सफलतापूर्वक प्राप्त हुआ!</h3>
            <p class="text-xs sm:text-sm text-brand-muted max-w-sm mx-auto">
              धन्यवाद! आपकी रसोई में शुद्ध, स्वादिष्ट अचार पहुँचाने की तैयारी शुरू हो चुकी है।
            </p>
            
            <div class="bg-brand-cream border border-brand-gold/40 px-4 py-2 rounded-xl inline-block font-mono font-bold text-brand-greendark text-sm">
              Order ID: #${orderId}
            </div>

            <div class="pt-2 space-y-2">
              <a href="https://wa.me/${PHONE}?text=${waMsg}" target="_blank" class="w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-3.5 px-6 rounded-xl flex items-center justify-center gap-2 shadow-md transition">
                <i class="fa-brands fa-whatsapp text-lg"></i>
                <span>WhatsApp पर तुरंत पर्ची भेजें</span>
              </a>

              <button onclick="clearAndCloseCart()" class="w-full bg-gray-100 hover:bg-gray-200 text-brand-earth font-bold py-3 rounded-xl text-xs transition">
                Continue Shopping (शॉपिंग जारी रखें)
              </button>
            </div>
          </div>
        `;

      } catch (err) {
        console.error("Order submit failed:", err);
        toast("Order failed: " + err.message, "error");
        btn.disabled = false;
        btn.innerHTML = `Order Place करें (₹${total})`;
      }
    }

    function clearAndCloseCart() {
      cart = [];
      saveCart();
      updateCartBadge();
      closeModal("cartModal");
      renderProducts();
    }

    /* ============================================================
       PAYMENT SETTINGS LOGIC
    ============================================================ */
    async function loadPaymentSettings() {
      if (!firebaseReady) {
        const cached = localStorage.getItem("mindo_payment");
        if (cached) paymentSettings = JSON.parse(cached);
        return;
      }
      try {
        const snapshot = await db.ref('settings/payment').once('value');
        if (snapshot.exists()) {
          paymentSettings = { ...paymentSettings, ...snapshot.val() };
        }
      } catch (e) {
        console.warn("Payment settings fetch error:", e);
      }
    }

    /* ============================================================
       ADMIN MANAGEMENT (AUTH, ORDERS, PRODUCTS, PAYMENTS)
    ============================================================ */
    function openAdmin() {
      const modal = document.getElementById("adminModal");
      modal.classList.remove("hidden");
      modal.classList.add("flex");
      document.body.style.overflow = "hidden";
      if (isAdmin) renderAdminDashboard();
      else renderAdminLogin();
    }

    function renderAdminLogin() {
      const container = document.getElementById("adminContent");
      container.innerHTML = `
        <div class="max-w-md mx-auto py-6 space-y-6">
          <div class="text-center space-y-2">
            <div class="w-12 h-12 mx-auto rounded-2xl bg-brand-green/10 text-brand-green flex items-center justify-center text-xl">
              <i class="fa-solid fa-shield-halved"></i>
            </div>
            <h2 class="font-serif font-black text-2xl text-brand-greendark">Mindo Admin Login</h2>
            <p class="text-xs text-brand-muted">सुरक्षित स्टोर मैनेजमेंट एवं ऑर्डर्स डैशबोर्ड</p>
          </div>

          <form onsubmit="adminLogin(event)" class="space-y-4">
            <div>
              <label class="block text-xs font-bold text-brand-earth mb-1">Admin Email</label>
              <input type="email" id="adminEmail" required placeholder="admin@example.com" class="w-full text-sm px-3.5 py-2.5 rounded-xl border border-gray-300 focus:border-brand-green outline-none">
            </div>

            <div>
              <label class="block text-xs font-bold text-brand-earth mb-1">Password</label>
              <input type="password" id="adminPass" required placeholder="••••••••" class="w-full text-sm px-3.5 py-2.5 rounded-xl border border-gray-300 focus:border-brand-green outline-none">
            </div>

            <button type="submit" id="loginBtn" class="w-full bg-brand-green hover:bg-brand-greendark text-white font-bold py-3 rounded-xl transition text-sm flex items-center justify-center gap-2">
              <span>Sign In as Admin</span>
            </button>
          </form>
        </div>
      `;
    }

    function adminLogin(e) {
      e.preventDefault();
      const email = document.getElementById("adminEmail").value.trim();
      const pass = document.getElementById("adminPass").value.trim();
      const btn = document.getElementById("loginBtn");

      btn.disabled = true;
      btn.innerHTML = `<i class="fa-solid fa-spinner animate-spin"></i> Authenticating...`;

      if (firebaseReady) {
        auth.signInWithEmailAndPassword(email, pass)
          .then(() => {
            toast("Welcome back Admin! 👋", "success");
            isAdmin = true;
            renderAdminDashboard();
          })
          .catch(err => {
            toast("Login Failed: " + err.message, "error");
            btn.disabled = false;
            btn.innerHTML = `Sign In as Admin`;
          });
      } else {
        // Simple offline fallback
        if (pass.length >= 4) {
          isAdmin = true;
          toast("Offline Admin Mode Activated", "success");
          renderAdminDashboard();
        } else {
          toast("Password should be at least 4 characters", "error");
          btn.disabled = false;
          btn.innerHTML = `Sign In as Admin`;
        }
      }
    }

    function renderAdminDashboard() {
      const container = document.getElementById("adminContent");
      container.innerHTML = `
        <div class="space-y-5">
          <div class="flex flex-wrap items-center justify-between pb-4 border-b border-gray-200 gap-2">
            <div>
              <h2 class="font-serif font-black text-2xl text-brand-greendark flex items-center gap-2">
                <i class="fa-solid fa-cubes-stacked text-brand-gold"></i> Admin Management
              </h2>
              <p class="text-xs text-brand-muted">Mindo Storefront Realtime Operations</p>
            </div>
            <button onclick="adminLogout()" class="text-xs font-bold px-3 py-1.5 rounded-lg border border-red-200 text-red-600 hover:bg-red-50 transition">
              <i class="fa-solid fa-arrow-right-from-bracket"></i> Logout
            </button>
          </div>

          <!-- Tab Navigation -->
          <div class="flex gap-2 border-b border-gray-100 pb-2">
            <button onclick="switchTab('orders')" class="px-4 py-2 rounded-xl text-xs font-bold transition ${adminTab === 'orders' ? 'bg-brand-green text-white' : 'text-gray-600 hover:bg-gray-100'}">
              <i class="fa-solid fa-box-open mr-1"></i> Customer Orders
            </button>
            <button onclick="switchTab('products')" class="px-4 py-2 rounded-xl text-xs font-bold transition ${adminTab === 'products' ? 'bg-brand-green text-white' : 'text-gray-600 hover:bg-gray-100'}">
              <i class="fa-solid fa-jar mr-1"></i> Products Catalog
            </button>
            <button onclick="switchTab('payment')" class="px-4 py-2 rounded-xl text-xs font-bold transition ${adminTab === 'payment' ? 'bg-brand-green text-white' : 'text-gray-600 hover:bg-gray-100'}">
              <i class="fa-solid fa-qrcode mr-1"></i> UPI & QR Settings
            </button>
          </div>

          <!-- Dynamic Panel Outlet -->
          <div id="adminPanelArea"></div>
        </div>
      `;
      renderAdminPanel();
    }

    function switchTab(tab) {
      adminTab = tab;
      renderAdminDashboard();
    }

    function renderAdminPanel() {
      const panel = document.getElementById("adminPanelArea");
      if (!panel) return;
      if (adminTab === "orders") renderOrdersPanel(panel);
      else if (adminTab === "products") renderProductsPanel(panel);
      else if (adminTab === "payment") renderPaymentPanel(panel);
    }

    /* ---- Orders Panel ---- */
    async function renderOrdersPanel(panel) {
      panel.innerHTML = `<div class="py-12 text-center text-gray-500"><i class="fa-solid fa-spinner animate-spin text-2xl"></i> Loading orders...</div>`;
      let orders = [];

      if (firebaseReady) {
        try {
          const snapshot = await db.ref('orders').once('value');
          const data = snapshot.val() || {};
          orders = Object.keys(data).map(key => ({ id: key, ...data[key] }));
          orders.sort((a, b) => (b.createdAt || 0) - (a.createdAt || 0));
        } catch (e) {
          toast("Error fetching orders: " + e.message, "error");
        }
      } else {
        orders = JSON.parse(localStorage.getItem("mindo_orders") || "[]");
        orders.reverse();
      }

      if (!orders.length) {
        panel.innerHTML = `
          <div class="text-center py-12 text-brand-muted bg-gray-50 rounded-2xl border border-dashed border-gray-200">
            <i class="fa-solid fa-inbox text-4xl block mb-2 opacity-40"></i>
            <p class="font-bold">अभी कोई ऑर्डर नहीं है</p>
          </div>
        `;
        return;
      }

      const pendingCount = orders.filter(o => o.status !== "delivered").length;

      const orderCards = orders.map(o => {
        const isDelivered = o.status === "delivered";
        const dateStr = new Date(o.createdAt || Date.now()).toLocaleString("en-IN", {
          day: "2-digit", month: "short", hour: "2-digit", minute: "2-digit"
        });
        const shortId = (o.id || "").slice(-6).toUpperCase();
        const itemsText = (o.items || []).map(i => `${i.name} × ${i.qty}`).join(", ");

        return `
          <div class="p-4 rounded-2xl border ${isDelivered ? 'bg-emerald-50/60 border-emerald-200' : 'bg-white border-gray-200 shadow-sm'} space-y-2">
            <div class="flex items-start justify-between gap-2">
              <div>
                <span class="font-mono text-xs font-bold text-brand-muted">#${shortId}</span>
                <h4 class="font-bold text-sm text-brand-greendark">${o.customerName} <span class="text-xs font-normal text-gray-500">(${dateStr})</span></h4>
                <p class="text-xs text-brand-earth font-medium"><i class="fa-solid fa-phone text-gray-400"></i> ${o.phone}</p>
              </div>
              <span class="text-[10px] uppercase font-extrabold px-2.5 py-1 rounded-full ${isDelivered ? 'bg-emerald-200 text-emerald-800' : 'bg-amber-100 text-amber-800'}">
                ${o.status || 'pending'}
              </span>
            </div>

            <div class="p-2.5 rounded-xl bg-gray-50 text-xs text-brand-earth border border-gray-100">
              <span class="font-bold text-brand-greendark">Jars:</span> ${itemsText}
            </div>

            <div class="text-xs text-gray-600">
              <p><span class="font-semibold text-gray-800">Address:</span> ${o.address}</p>
              ${o.note ? `<p><span class="font-semibold text-gray-800">Note:</span> ${o.note}</p>` : ''}
              <p class="mt-1 font-serif font-black text-sm text-brand-red">Total: ₹${o.total}</p>
            </div>

            <div class="pt-2 flex flex-wrap items-center gap-2 border-t border-gray-100">
              ${!isDelivered ? `
                <button onclick="markOrderStatus('${o.id}', 'delivered')" class="bg-emerald-600 hover:bg-emerald-700 text-white text-xs font-bold px-3 py-1.5 rounded-lg flex items-center gap-1">
                  <i class="fa-solid fa-check"></i> Mark Delivered
                </button>
              ` : `
                <button onclick="markOrderStatus('${o.id}', 'pending')" class="bg-gray-200 hover:bg-gray-300 text-gray-700 text-xs font-bold px-3 py-1.5 rounded-lg">
                  ↩ Undo to Pending
                </button>
              `}

              <a href="https://wa.me/91${o.phone}?text=${encodeURIComponent('Namaste ' + o.customerName + '! Your Mindo Pickles order #' + shortId + ' is processed.')}" target="_blank" class="text-xs font-bold px-3 py-1.5 rounded-lg bg-green-50 text-emerald-700 border border-green-200 hover:bg-green-100">
                <i class="fa-brands fa-whatsapp"></i> WhatsApp
              </a>

              <a href="tel:${o.phone}" class="text-xs font-bold px-3 py-1.5 rounded-lg bg-gray-100 text-gray-700 hover:bg-gray-200">
                <i class="fa-solid fa-phone"></i> Call
              </a>
            </div>
          </div>
        `;
      }).join("");

      panel.innerHTML = `
        <div class="space-y-4">
          <div class="flex items-center justify-between">
            <span class="text-xs font-bold text-brand-greendark">Total: ${orders.length} | Pending: ${pendingCount}</span>
            <button onclick="renderAdminPanel()" class="text-xs font-bold text-brand-green hover:underline flex items-center gap-1">
              <i class="fa-solid fa-arrows-rotate"></i> Refresh
            </button>
          </div>
          <div class="max-h-[55vh] overflow-y-auto space-y-3 pr-1">
            ${orderCards}
          </div>
        </div>
      `;
    }

    async function markOrderStatus(id, status) {
      try {
        if (firebaseReady) {
          await db.ref('orders/' + id).update({
            status: status,
            updatedAt: firebase.database.ServerValue.TIMESTAMP
          });
        } else {
          const orders = JSON.parse(localStorage.getItem("mindo_orders") || "[]");
          const target = orders.find(x => x.id === id);
          if (target) target.status = status;
          localStorage.setItem("mindo_orders", JSON.stringify(orders));
        }
        toast(`Order updated to ${status}`);
        renderAdminPanel();
      } catch (err) {
        toast("Status update error: " + err.message, "error");
      }
    }

    /* ---- Products Panel ---- */
    function renderProductsPanel(panel) {
      const itemsList = products.map((p, idx) => `
        <div class="flex items-center justify-between p-3 rounded-xl bg-white border border-gray-200 gap-3">
          <div class="flex items-center gap-3">
            <span class="text-2xl">${p.emoji || "🫙"}</span>
            <div>
              <h4 class="font-bold text-xs sm:text-sm text-brand-greendark">${p.name}</h4>
              <p class="text-xs text-brand-red font-semibold">₹${p.price} ${p.mrp ? `<span class="text-gray-400 line-through">₹${p.mrp}</span>` : ''} ${p.bestseller ? '• ⭐ Bestseller' : ''}</p>
            </div>
          </div>
          <div class="flex items-center gap-2">
            <button onclick="openProductFormModal(${idx})" class="w-8 h-8 rounded-lg bg-gray-100 hover:bg-brand-green hover:text-white text-gray-700 flex items-center justify-center text-xs transition">
              <i class="fa-solid fa-pen"></i>
            </button>
            <button onclick="deleteProduct(${idx})" class="w-8 h-8 rounded-lg bg-gray-100 hover:bg-brand-red hover:text-white text-gray-700 flex items-center justify-center text-xs transition">
              <i class="fa-solid fa-trash"></i>
            </button>
          </div>
        </div>
      `).join("");

      panel.innerHTML = `
        <div class="space-y-4">
          <div class="flex items-center justify-between">
            <span class="text-xs font-bold text-brand-greendark">${products.length} Products listed</span>
            <button onclick="openProductFormModal(-1)" class="bg-brand-green hover:bg-brand-greendark text-white text-xs font-bold px-3 py-1.5 rounded-lg flex items-center gap-1 transition">
              <i class="fa-solid fa-plus"></i> Add New Pickle
            </button>
          </div>
          <div class="max-h-[45vh] overflow-y-auto space-y-2 pr-1">
            ${itemsList || '<p class="text-xs text-gray-400">No products</p>'}
          </div>
          <div id="productFormArea"></div>
        </div>
      `;
    }

    function openProductFormModal(index = -1) {
      const p = index >= 0 ? products[index] : {
        name: "", hi: "", tag: "", price: 249, mrp: 299, emoji: "🫙", img: "", bestseller: false
      };

      const container = document.getElementById("productFormArea");
      container.innerHTML = `
        <div class="p-4 rounded-2xl bg-amber-50/70 border border-brand-gold/40 mt-3 space-y-3">
          <h4 class="font-serif font-black text-sm text-brand-greendark">
            ${index >= 0 ? 'Edit Pickle Details' : 'Add New Handcrafted Pickle'}
          </h4>

          <form onsubmit="saveProduct(event, ${index})" class="space-y-3 text-xs">
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-2">
              <div>
                <label class="block font-bold mb-1">Pickle English Name *</label>
                <input name="name" required value="${p.name || ''}" placeholder="e.g. Aam Ka Achar" class="w-full p-2 rounded-lg border border-gray-300">
              </div>
              <div>
                <label class="block font-bold mb-1">Hindi Display Name</label>
                <input name="hi" value="${p.hi || ''}" placeholder="जैसे: दादी का आम अचार" class="w-full p-2 rounded-lg border border-gray-300">
              </div>
            </div>

            <div>
              <label class="block font-bold mb-1">Short Description / Spices</label>
              <input name="tag" value="${p.tag || ''}" placeholder="e.g. 100% सरसों तेल, सौंफ व मेथी के साथ" class="w-full p-2 rounded-lg border border-gray-300">
            </div>

            <div class="grid grid-cols-2 sm:grid-cols-3 gap-2">
              <div>
                <label class="block font-bold mb-1">Selling Price (₹) *</label>
                <input type="number" name="price" required value="${p.price || ''}" class="w-full p-2 rounded-lg border border-gray-300">
              </div>
              <div>
                <label class="block font-bold mb-1">MRP (₹)</label>
                <input type="number" name="mrp" value="${p.mrp || ''}" class="w-full p-2 rounded-lg border border-gray-300">
              </div>
              <div>
                <label class="block font-bold mb-1">Emoji Icon</label>
                <input name="emoji" maxlength="4" value="${p.emoji || '🫙'}" class="w-full p-2 rounded-lg border border-gray-300 text-center">
              </div>
            </div>

            <div>
              <label class="block font-bold mb-1">Upload Product Photo (Canvas Compressed)</label>
              <input type="file" accept="image/*" onchange="handleProductImageUpload(event)" class="w-full text-xs">
              <input type="hidden" name="img" id="productImageBase64" value="${p.img || ''}">
              <div id="productImgPreview" class="mt-2">
                ${p.img ? `<img src="${p.img}" class="h-16 rounded-lg border border-gray-200">` : ''}
              </div>
            </div>

            <div class="flex items-center gap-2 pt-1">
              <input type="checkbox" id="bestsellerCheck" name="bestseller" ${p.bestseller ? 'checked' : ''}>
              <label for="bestsellerCheck" class="font-bold cursor-pointer">Mark as ⭐ Bestseller badge</label>
            </div>

            <div class="flex items-center gap-2 pt-2">
              <button type="submit" class="bg-brand-green text-white font-bold px-4 py-2 rounded-lg text-xs hover:bg-brand-greendark">Save Pickle</button>
              <button type="button" onclick="document.getElementById('productFormArea').innerHTML=''" class="bg-gray-200 text-gray-700 font-bold px-4 py-2 rounded-lg text-xs">Cancel</button>
            </div>
          </form>
        </div>
      `;
    }

    function handleProductImageUpload(e) {
      const file = e.target.files[0];
      if (!file) return;

      const reader = new FileReader();
      reader.onload = function (event) {
        const img = new Image();
        img.onload = function () {
          const canvas = document.createElement('canvas');
          const MAX_WIDTH = 450;
          const scale = MAX_WIDTH / img.width;
          canvas.width = MAX_WIDTH;
          canvas.height = img.height * scale;
          const ctx = canvas.getContext('2d');
          ctx.drawImage(img, 0, 0, canvas.width, canvas.height);

          const compressed = canvas.toDataURL('image/jpeg', 0.75);
          document.getElementById('productImageBase64').value = compressed;
          document.getElementById('productImgPreview').innerHTML = `<img src="${compressed}" class="h-16 rounded-lg border border-gray-300 shadow-sm">`;
        };
        img.src = event.target.result;
      };
      reader.readAsDataURL(file);
    }

    async function saveProduct(e, index) {
      e.preventDefault();
      const fd = new FormData(e.target);
      const data = {
        name: fd.get("name").trim(),
        hi: fd.get("hi").trim(),
        tag: fd.get("tag").trim(),
        price: parseInt(fd.get("price")),
        mrp: parseInt(fd.get("mrp")) || null,
        emoji: fd.get("emoji").trim() || "🫙",
        img: fd.get("img").trim(),
        bestseller: fd.get("bestseller") === "on"
      };

      try {
        if (firebaseReady) {
          if (index >= 0 && products[index].id && !products[index].id.startsWith("local_")) {
            await db.ref('products/' + products[index].id).update(data);
          } else {
            const newRef = await db.ref('products').push({
              ...data,
              createdAt: firebase.database.ServerValue.TIMESTAMP
            });
            data.id = newRef.key;
          }
        }

        if (index >= 0) products[index] = { ...products[index], ...data };
        else products.push({ id: "local_" + Date.now(), ...data });

        localStorage.setItem("mindo_products_new", JSON.stringify(products));
        toast("✅ Pickle Saved!", "success");
        renderProducts();
        renderAdminPanel();
      } catch (err) {
        toast("Failed to save: " + err.message, "error");
      }
    }

    async function deleteProduct(index) {
      const p = products[index];
      if (!p) return;

      // Safe non-blocking custom modal or straightforward confirmation
      const proceed = window.confirm ? confirm(`Delete '${p.name}' from pickle catalog?`) : true;
      if (!proceed) return;

      try {
        if (firebaseReady && p.id && !p.id.startsWith("local_")) {
          await db.ref('products/' + p.id).remove();
        }
        products.splice(index, 1);
        localStorage.setItem("mindo_products_new", JSON.stringify(products));
        toast("Pickle removed", "success");
        renderProducts();
        renderAdminPanel();
      } catch (err) {
        toast("Deletion error: " + err.message, "error");
      }
    }

    /* ---- Payment Settings Panel ---- */
    function renderPaymentPanel(panel) {
      panel.innerHTML = `
        <div class="p-4 rounded-2xl bg-amber-50/70 border border-brand-gold/30 space-y-4">
          <h4 class="font-serif font-black text-sm text-brand-greendark">Payment & UPI Setup</h4>
          
          <div class="space-y-3">
            <div>
              <label class="block text-xs font-bold text-brand-earth mb-1">Your Business UPI ID (VPA)</label>
              <input type="text" id="upiIdInput" value="${paymentSettings.upiId || ''}" placeholder="e.g. 8383050500@ybl" class="w-full text-xs sm:text-sm p-2.5 rounded-lg border border-gray-300">
            </div>

            <div>
              <label class="block text-xs font-bold text-brand-earth mb-1">Custom Store QR Code Image (Optional)</label>
              <input type="file" accept="image/*" onchange="handleQrUpload(event)" class="text-xs">
              <div id="qrPreviewArea" class="mt-2">
                ${paymentSettings.qrCode ? `<img src="${paymentSettings.qrCode}" class="w-28 h-28 object-contain rounded-lg border border-amber-300 p-1 bg-white">` : ''}
              </div>
            </div>

            <button onclick="saveUpiSettings()" class="bg-brand-green text-white font-bold px-4 py-2.5 rounded-lg text-xs hover:bg-brand-greendark transition">
              <i class="fa-solid fa-floppy-disk mr-1"></i> Save Payment Config
            </button>
          </div>
        </div>
      `;
    }

    function handleQrUpload(e) {
      const file = e.target.files[0];
      if (!file) return;

      const reader = new FileReader();
      reader.onload = function (ev) {
        paymentSettings.qrCode = ev.target.result;
        document.getElementById('qrPreviewArea').innerHTML = `<img src="${ev.target.result}" class="w-28 h-28 object-contain rounded-lg border border-amber-300 p-1 bg-white">`;
      };
      reader.readAsDataURL(file);
    }

    async function saveUpiSettings() {
      const upiId = document.getElementById("upiIdInput").value.trim();
      paymentSettings.upiId = upiId;

      try {
        if (firebaseReady) {
          await db.ref('settings/payment').update({
            upiId: paymentSettings.upiId,
            qrCode: paymentSettings.qrCode || "",
            updatedAt: firebase.database.ServerValue.TIMESTAMP
          });
        }
        localStorage.setItem("mindo_payment", JSON.stringify(paymentSettings));
        toast("✅ UPI Details saved successfully!", "success");
      } catch (err) {
        toast("Save error: " + err.message, "error");
      }
    }

    function adminLogout() {
      if (firebaseReady && auth) {
        auth.signOut().then(() => {
          isAdmin = false;
          closeModal("adminModal");
          toast("Logged out securely");
        });
      } else {
        isAdmin = false;
        closeModal("adminModal");
        toast("Logged out");
      }
    }

    /* ============================================================
       HELPER UTILS & TOAST
    ============================================================ */
    function closeModal(id) {
      const el = document.getElementById(id);
      if (el) {
        el.classList.add("hidden");
        el.classList.remove("flex");
      }
      document.body.style.overflow = "";
    }

    function toast(msg, type = "success") {
      const t = document.getElementById("toast");
      if (!t) return;
      t.innerHTML = `<span>${msg}</span>`;
      t.classList.remove("opacity-0", "-translate-y-4");
      t.classList.add("opacity-100", "translate-y-0");

      if (type === "error") {
        t.classList.add("bg-brand-red");
        t.classList.remove("bg-brand-earth");
      } else {
        t.classList.remove("bg-brand-red");
        t.classList.add("bg-brand-earth");
      }

      clearTimeout(t._timer);
      t._timer = setTimeout(() => {
        t.classList.remove("opacity-100", "translate-y-0");
        t.classList.add("opacity-0", "-translate-y-4");
      }, 3200);
    }

    // Modal background click close guard
    document.querySelectorAll('#cartModal, #adminModal').forEach(modal => {
      modal.addEventListener('click', (e) => {
        if (e.target === modal) closeModal(modal.id);
      });
    });

    // Boot up
    window.addEventListener("DOMContentLoaded", init);
  </script>
</body>
</html>
```