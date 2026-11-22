# KustomDetailzMobile
<!DOCTYPE html>
<html lang="en" class="scroll-smooth dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>KustomDetailz | Detail • Protect • Shine — We Come To You!</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Plus+Jakarta+Sans:wght@600;700;800&display=swap" rel="stylesheet" />

  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
            display: ['Plus Jakarta Sans', 'sans-serif'],
          },
          colors: {
            brand: {
              DEFAULT: 'var(--accent-primary)',
              hover: 'var(--accent-hover)',
              glow: 'var(--accent-glow)',
              soft: 'var(--accent-soft)',
            }
          }
        }
      }
    };
  </script>

  <style>
    /* Theme variables matched to KustomDetailz Gold, Chrome & Sunset Amber palette */
    :root {
      --accent-primary: #f59e0b;
      --accent-hover: #d97706;
      --accent-glow: rgba(245, 158, 11, 0.35);
      --accent-soft: rgba(245, 158, 11, 0.14);
      --sunset-secondary: #ea580c;
    }

    body {
      background-color: #09090b;
      color: #f4f4f5;
      overflow-x: hidden;
    }

    /* Metallic chrome and gold text effects */
    .text-chrome-gradient {
      background: linear-gradient(180deg, #ffffff 0%, #e4e4e7 48%, #9ca3af 52%, #f4f4f5 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .text-gold-gradient {
      background: linear-gradient(180deg, #fef08a 0%, #f59e0b 48%, #b45309 54%, #fbbf24 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    /* Subtle grid backdrop */
    .bg-grid-pattern {
      background-size: 40px 40px;
      background-image:
        linear-gradient(to right, rgba(245, 158, 11, 0.04) 1px, transparent 1px),
        linear-gradient(to bottom, rgba(245, 158, 11, 0.04) 1px, transparent 1px);
    }

    /* Glass header bar */
    .glass-nav {
      background: rgba(9, 9, 11, 0.88);
      backdrop-filter: blur(14px);
      -webkit-backdrop-filter: blur(14px);
      border-bottom: 1px solid rgba(245, 158, 11, 0.18);
    }

    /* Card surface */
    .metallic-card {
      background: linear-gradient(145deg, rgba(28, 28, 34, 0.94) 0%, rgba(15, 15, 19, 0.97) 100%);
      border: 1px solid rgba(255, 255, 255, 0.09);
      box-shadow: 0 20px 40px -15px rgba(0, 0, 0, 0.7);
    }

    .metallic-card:hover {
      border-color: rgba(245, 158, 11, 0.34);
    }

    /* Before/After range slider styling */
    .comparison-slider {
      -webkit-appearance: none;
      appearance: none;
      background: transparent;
      cursor: ew-resize;
    }

    .comparison-slider::-webkit-slider-thumb {
      -webkit-appearance: none;
      appearance: none;
      width: 42px;
      height: 42px;
      border-radius: 9999px;
      background: #ffffff;
      border: 3px solid var(--accent-primary);
      box-shadow: 0 4px 16px rgba(0, 0, 0, 0.55);
      cursor: ew-resize;
    }

    .comparison-slider::-moz-range-thumb {
      width: 42px;
      height: 42px;
      border-radius: 9999px;
      background: #ffffff;
      border: 3px solid var(--accent-primary);
      box-shadow: 0 4px 16px rgba(0, 0, 0, 0.55);
      cursor: ew-resize;
    }
  </style>
</head>

<body class="bg-grid-pattern antialiased selection:bg-amber-500 selection:text-black">

  <!-- STICKY TOP NAVIGATION -->
  <header class="glass-nav sticky top-0 z-40">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-20">
        <!-- Brand Logo with Image + SVG Emblem Fallback -->
        <a href="#" class="flex items-center gap-3 group">
          <div class="h-12 w-20 sm:w-24 rounded-xl overflow-hidden border border-amber-400/40 bg-black flex items-center justify-center shadow-lg transition-transform group-hover:scale-105 shrink-0" style="box-shadow: 0 0 18px var(--accent-glow);">
            <img
              data-logo-img
              src="./image_1277c7.jpg"
              alt="KustomDetailz Logo"
              onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
              class="w-full h-full object-cover"
            />
            <!-- Crisp SVG Car Emblem Fallback (shown automatically if image isn't loaded) -->
            <div class="hidden w-full h-full items-center justify-center px-1.5 bg-gradient-to-br from-zinc-950 via-zinc-900 to-amber-950/50">
              <svg viewBox="0 0 140 64" class="w-full h-full" aria-label="KustomDetailz Emblem">
                <defs>
                  <linearGradient id="kdGoldNav" x1="0%" y1="0%" x2="0%" y2="100%">
                    <stop offset="0%" stop-color="#fef08a" />
                    <stop offset="50%" stop-color="#f59e0b" />
                    <stop offset="100%" stop-color="#b45309" />
                  </linearGradient>
                  <linearGradient id="kdChromeNav" x1="0%" y1="0%" x2="0%" y2="100%">
                    <stop offset="0%" stop-color="#ffffff" />
                    <stop offset="50%" stop-color="#d4d4d8" />
                    <stop offset="100%" stop-color="#71717a" />
                  </linearGradient>
                </defs>
                <path d="M16 36 C24 20, 48 14, 76 14 C102 14, 118 22, 128 33 L116 36 C104 28, 86 24, 62 24 C42 24, 28 29, 16 36 Z" fill="url(#kdGoldNav)" />
                <text x="70" y="45" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="800" font-style="italic" font-size="14" fill="url(#kdChromeNav)">KUSTOM</text>
                <text x="70" y="58" text-anchor="middle" font-family="Inter, sans-serif" font-weight="800" font-size="7.5" letter-spacing="1.4" fill="url(#kdGoldNav)">DETAIL • PROTECT • SHINE</text>
              </svg>
            </div>
          </div>
          <div>
            <span class="font-display font-extrabold text-xl sm:text-2xl tracking-tight block leading-none">
              <span class="text-chrome-gradient">Kustom</span><span class="text-gold-gradient">Detailz</span>
            </span>
            <span class="text-[10px] font-bold tracking-[0.18em] text-amber-400/90 uppercase block mt-1">
              DETAIL • PROTECT • SHINE
            </span>
          </div>
        </a>

        <!-- Desktop Navigation Links -->
        <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-zinc-300">
          <a href="#services" class="hover:text-amber-400 transition-colors">Services &amp; Pricing</a>
          <a href="#results" class="hover:text-amber-400 transition-colors">Before &amp; After</a>
          <a href="#booking" class="hover:text-amber-400 transition-colors">Book Now</a>
        </nav>

        <!-- Call & Book CTA -->
        <div class="hidden sm:flex items-center gap-3">
          <a
            href="tel:+17124908490"
            class="px-3.5 py-2.5 rounded-xl text-xs font-semibold text-zinc-200 border border-white/15 bg-zinc-900/80 hover:border-amber-400/50 hover:text-amber-300 transition-all"
          >
            (712) 490-8490
          </a>
          <a
            href="#booking"
            class="px-5 py-2.5 rounded-xl text-sm font-bold text-black transition-all transform hover:-translate-y-0.5"
            style="background: linear-gradient(135deg, #fde047 0%, var(--accent-primary) 55%, var(--sunset-secondary) 100%); box-shadow: 0 6px 20px var(--accent-glow);"
          >
            Book Mobile Detail
          </a>
        </div>

        <!-- Mobile Menu Button -->
        <button
          id="mobile-menu-btn"
          type="button"
          aria-label="Toggle navigation menu"
          class="md:hidden p-2.5 rounded-xl text-zinc-300 hover:text-white hover:bg-white/10 transition-colors"
        >
          <svg id="menu-icon-open" class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
          <svg id="menu-icon-close" class="w-6 h-6 hidden" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
      </div>
    </div>

    <!-- Mobile Dropdown Menu -->
    <div id="mobile-menu" class="hidden md:hidden border-t border-white/10 bg-zinc-950/95 px-4 py-5 space-y-3">
      <a href="#services" class="mobile-nav-link block py-2.5 px-3 rounded-lg text-base font-medium text-zinc-200 hover:bg-white/5">Services &amp; Pricing</a>
      <a href="#results" class="mobile-nav-link block py-2.5 px-3 rounded-lg text-base font-medium text-zinc-200 hover:bg-white/5">Before &amp; After</a>
      <a href="#booking" class="mobile-nav-link block py-2.5 px-3 rounded-lg text-base font-medium text-zinc-200 hover:bg-white/5">Book Now</a>
      <div class="pt-3 border-t border-white/10 flex flex-col gap-2.5">
        <a
          href="tel:+17124908490"
          class="w-full text-center py-3 px-4 rounded-xl font-semibold text-sm text-amber-300 border border-amber-400/35 bg-amber-500/10"
        >
          Call or Text (712) 490-8490
        </a>
        <a
          href="#booking"
          class="mobile-nav-link block w-full text-center py-3 px-4 rounded-xl font-bold text-sm text-black"
          style="background: linear-gradient(135deg, #fde047 0%, var(--accent-primary) 60%, var(--sunset-secondary) 100%);"
        >
          Get Instant Estimate &amp; Book
        </a>
      </div>
    </div>
  </header>

  <!-- HERO SECTION -->
  <section class="relative pt-12 pb-20 lg:pt-20 lg:pb-28 overflow-hidden">
    <!-- Ambient sunset and gold glow orbs -->
    <div class="absolute -top-24 left-1/2 -translate-x-1/2 w-[780px] h-[380px] rounded-full blur-[135px] pointer-events-none opacity-30" style="background: radial-gradient(circle, var(--accent-primary), var(--sunset-secondary));"></div>

    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
      <div class="grid lg:grid-cols-12 gap-12 items-center">

        <!-- Hero Copy -->
        <div class="lg:col-span-6 text-center lg:text-left">
          <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full text-xs font-bold tracking-wider uppercase mb-6 border border-amber-400/35 bg-amber-500/10 text-amber-300">
            <span class="w-2 h-2 rounded-full bg-amber-400 animate-pulse"></span>
            DETAIL • PROTECT • SHINE • WE COME TO YOU!
          </div>

          <h1 class="font-display text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight leading-[1.08] mb-6">
            <span class="text-chrome-gradient">Kustom</span><span class="text-gold-gradient">Detailz</span><br />
            <span class="text-white">Mobile Detailing.</span>
          </h1>

          <p class="text-base sm:text-lg text-zinc-300 max-w-xl mx-auto lg:mx-0 mb-8 leading-relaxed">
            From deep interior refreshes and gloss-boosting paint polishing to crystal-clear headlight restoration, we bring professional care straight to your driveway or workplace.
          </p>

          <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4">
            <a
              href="#booking"
              class="w-full sm:w-auto px-7 py-4 rounded-2xl font-bold text-base text-black transition-all transform hover:-translate-y-0.5 text-center"
              style="background: linear-gradient(135deg, #fde047 0%, var(--accent-primary) 55%, var(--sunset-secondary) 100%); box-shadow: 0 10px 28px var(--accent-glow);"
            >
              Book Your Detail
            </a>
            <a
              href="#services"
              class="w-full sm:w-auto px-7 py-4 rounded-2xl font-semibold text-base text-white bg-white/5 hover:bg-white/10 border border-white/15 transition-all text-center"
            >
              Explore Services
            </a>
          </div>
        </div>

        <!-- Logo Showcase Card -->
        <div class="lg:col-span-6">
          <div class="metallic-card rounded-3xl p-4 sm:p-6 relative overflow-hidden border border-amber-500/25">
            <div class="relative aspect-[16/10] rounded-2xl overflow-hidden border border-amber-400/35 shadow-2xl bg-black flex items-center justify-center">
              <img
                data-logo-img
                src="./image_1277c7.jpg"
                alt="KustomDetailz — Detail, Protect, Shine"
                onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
                class="w-full h-full object-cover"
              />
              <!-- Self-Contained SVG Car Emblem Fallback -->
              <div class="hidden w-full h-full flex-col items-center justify-center p-6 text-center bg-gradient-to-br from-zinc-950 via-zinc-900 to-amber-950/60">
                <svg viewBox="0 0 320 120" class="w-full max-w-sm h-auto mb-2" aria-label="KustomDetailz Emblem Showcase">
                  <defs>
                    <linearGradient id="kdGoldHero" x1="0%" y1="0%" x2="0%" y2="100%">
                      <stop offset="0%" stop-color="#fef08a" />
                      <stop offset="50%" stop-color="#f59e0b" />
                      <stop offset="100%" stop-color="#b45309" />
                    </linearGradient>
                    <linearGradient id="kdChromeHero" x1="0%" y1="0%" x2="0%" y2="100%">
                      <stop offset="0%" stop-color="#ffffff" />
                      <stop offset="48%" stop-color="#e4e4e7" />
                      <stop offset="52%" stop-color="#9ca3af" />
                      <stop offset="100%" stop-color="#f4f4f5" />
                    </linearGradient>
                  </defs>
                  <path d="M32 68 C52 34, 108 20, 174 20 C236 20, 274 36, 294 60 L264 66 C238 48, 198 40, 146 40 C98 40, 62 50, 32 68 Z" fill="url(#kdGoldHero)" />
                  <text x="160" y="84" text-anchor="middle" font-family="Plus Jakarta Sans, sans-serif" font-weight="800" font-style="italic" font-size="30" fill="url(#kdChromeHero)">KustomDetailz</text>
                  <text x="160" y="106" text-anchor="middle" font-family="Inter, sans-serif" font-weight="800" font-size="13" letter-spacing="3.5" fill="url(#kdGoldHero)">DETAIL • PROTECT • SHINE</text>
                </svg>
                <span class="text-xs text-zinc-400">
                  Tip: Place <code class="text-amber-300">image_1277c7.jpg</code> next to <code class="text-amber-300">index.html</code> or set <code class="text-amber-300">SITE_CONFIG.logoImageUrl</code> to a direct URL.
                </span>
              </div>
              <div class="absolute inset-0 ring-1 ring-inset ring-white/10 rounded-2xl pointer-events-none"></div>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- SERVICES & PRICING SECTION -->
  <section id="services" class="py-20 lg:py-28 border-t border-white/10 bg-zinc-950/50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center max-w-3xl mx-auto mb-10">
        <span class="text-xs font-bold uppercase tracking-widest text-amber-400">Mobile Detailing Menu • We Come To You!</span>
        <h2 class="font-display text-3xl sm:text-4xl lg:text-5xl font-extrabold mt-2 mb-4">
          Services Built for <span class="text-gold-gradient">Every Detail</span>
        </h2>
        <p class="text-zinc-400 text-base sm:text-lg">
          Select your vehicle size below to preview estimated pricing, then open any full checklist or jump straight into your booking estimate.
        </p>
      </div>

      <!-- Vehicle Size Selector Pills -->
      <div class="flex flex-col items-center mb-12">
        <span class="text-xs font-semibold uppercase tracking-wider text-zinc-400 mb-3">Select Vehicle Size</span>
        <div id="vehicle-size-selector" class="inline-flex flex-wrap justify-center gap-2 p-1.5 rounded-2xl bg-zinc-900 border border-white/10">
          <button type="button" data-size="sedan" class="vehicle-btn px-4 py-2.5 rounded-xl text-sm font-semibold transition-all">
            Coupe / Sedan <span class="text-xs opacity-75 ml-1">(Base)</span>
          </button>
          <button type="button" data-size="suv" class="vehicle-btn px-4 py-2.5 rounded-xl text-sm font-semibold transition-all">
            Mid-Size / 2-Row SUV <span class="text-xs opacity-75 ml-1">(+$25)</span>
          </button>
          <button type="button" data-size="truck" class="vehicle-btn px-4 py-2.5 rounded-xl text-sm font-semibold transition-all">
            Truck / 3-Row SUV <span class="text-xs opacity-75 ml-1">(+$50)</span>
          </button>
        </div>
      </div>

      <!-- Services Grid (Populated dynamically by JavaScript from SITE_CONFIG) -->
      <div id="services-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-7 items-stretch"></div>
    </div>
  </section>

  <!-- INTERACTIVE BEFORE & AFTER COMPARISON -->
  <section id="results" class="py-20 lg:py-28 border-t border-white/10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid lg:grid-cols-12 gap-12 items-center">
        <div class="lg:col-span-5">
          <span class="text-xs font-bold uppercase tracking-widest text-amber-400">Finish &amp; Clarity</span>
          <h2 class="font-display text-3xl sm:text-4xl font-extrabold mt-2 mb-4">
            See the <span class="text-chrome-gradient">Difference</span> Up Close
          </h2>
          <p class="text-zinc-400 text-base leading-relaxed mb-6">
            Drag the slider across the panel to compare dull, weathered paint and haze against a freshly polished, sealed finish. Every KustomDetailz session finishes with a careful final inspection.
          </p>
          <ul class="space-y-3 text-sm text-zinc-300">
            <li class="flex items-center gap-2.5">
              <span class="w-2 h-2 rounded-full bg-amber-400"></span>
              Paint-safe wash, decontamination &amp; sealant protection
            </li>
            <li class="flex items-center gap-2.5">
              <span class="w-2 h-2 rounded-full bg-amber-400"></span>
              Oxidation &amp; haze removal on cloudy headlights
            </li>
            <li class="flex items-center gap-2.5">
              <span class="w-2 h-2 rounded-full bg-amber-400"></span>
              Mobile convenience at your home or workplace
            </li>
          </ul>
        </div>

        <div class="lg:col-span-7">
          <div class="metallic-card rounded-3xl p-3 sm:p-4">
            <div class="relative aspect-[16/10] rounded-2xl overflow-hidden select-none bg-zinc-900">
              <!-- After Layer (Full width underneath) -->
              <div class="absolute inset-0 flex flex-col justify-between p-6 sm:p-8 bg-gradient-to-br from-amber-500/25 via-zinc-900 to-orange-600/25">
                <div class="flex justify-between items-start">
                  <span class="px-3 py-1 rounded-full text-xs font-bold uppercase tracking-wider bg-amber-400 text-black">After: Polished &amp; Sealed</span>
                  <span class="text-xs font-semibold text-amber-200 bg-black/50 px-3 py-1 rounded-full">Deep Gloss</span>
                </div>
                <div class="bg-black/60 backdrop-blur-sm border border-amber-400/30 rounded-2xl p-4 sm:p-5 max-w-md">
                  <p class="font-display font-bold text-lg text-white">Crisp Reflections &amp; Protection</p>
                  <p class="text-xs sm:text-sm text-zinc-300 mt-1">Smooth paint feel, rich trim &amp; tire dressing, and a durable sealant layer built to shine.</p>
                </div>
              </div>

              <!-- Before Layer (Clipped dynamically by slider percentage) -->
              <div id="before-layer" class="absolute inset-0 flex flex-col justify-between p-6 sm:p-8 bg-gradient-to-br from-zinc-800 via-zinc-900 to-stone-900" style="clip-path: inset(0 50% 0 0);">
                <div class="flex justify-between items-start">
                  <span class="px-3 py-1 rounded-full text-xs font-bold uppercase tracking-wider bg-zinc-700 text-zinc-100">Before: Dull &amp; Weathered</span>
                </div>
                <div class="bg-zinc-950/75 border border-white/10 rounded-2xl p-4 sm:p-5 max-w-md">
                  <p class="font-display font-bold text-lg text-zinc-200">Road Grime, Haze &amp; Buildup</p>
                  <p class="text-xs sm:text-sm text-zinc-400 mt-1">Everyday dust, water spots, oxidation, and muted reflections before detailing.</p>
                </div>
              </div>

              <!-- Divider Line -->
              <div id="comparison-divider" class="absolute top-0 bottom-0 w-0.5 bg-amber-300 shadow-[0_0_12px_rgba(251,191,36,0.9)] pointer-events-none" style="left: 50%;"></div>

              <!-- Interactive Range Input -->
              <input
                id="comparison-range"
                type="range"
                min="5"
                max="95"
                value="50"
                aria-label="Compare before and after detailing finish"
                class="comparison-slider absolute inset-0 w-full h-full opacity-0 z-20"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- LIVE BOOKING & QUOTE ESTIMATOR -->
  <section id="booking" class="py-20 lg:py-28 border-t border-white/10 bg-zinc-950/60">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center max-w-2xl mx-auto mb-12">
        <span class="text-xs font-bold uppercase tracking-widest text-amber-400">Mobile Service • We Come To You!</span>
        <h2 class="font-display text-3xl sm:text-4xl lg:text-5xl font-extrabold mt-2 mb-3">
          Instant Estimate &amp; <span class="text-gold-gradient">Booking</span>
        </h2>
        <p class="text-zinc-400 text-base">
          Build your service request below or call/text <a href="tel:+17124908490" class="text-amber-300 font-semibold hover:underline">(712) 490-8490</a> for direct scheduling.
        </p>
      </div>

      <div class="grid lg:grid-cols-12 gap-8 items-start">
        <!-- Booking Form -->
        <form id="booking-form" class="lg:col-span-7 metallic-card rounded-3xl p-6 sm:p-8 space-y-6">
          <div class="grid sm:grid-cols-2 gap-5">
            <div>
              <label for="customer-name" class="block text-xs font-bold uppercase tracking-wider text-zinc-300 mb-2">Your Name *</label>
              <input
                id="customer-name"
                type="text"
                required
                placeholder="Alex Rivera"
                class="w-full px-4 py-3 rounded-xl bg-zinc-900/90 border border-white/15 text-white placeholder-zinc-500 focus:outline-none focus:border-amber-400"
              />
            </div>
            <div>
              <label for="customer-phone" class="block text-xs font-bold uppercase tracking-wider text-zinc-300 mb-2">Phone Number *</label>
              <input
                id="customer-phone"
                type="tel"
                required
                placeholder="(712) 555-0199"
                class="w-full px-4 py-3 rounded-xl bg-zinc-900/90 border border-white/15 text-white placeholder-zinc-500 focus:outline-none focus:border-amber-400"
              />
            </div>
          </div>

          <div class="grid sm:grid-cols-2 gap-5">
            <div>
              <label for="booking-service" class="block text-xs font-bold uppercase tracking-wider text-zinc-300 mb-2">Primary Service</label>
              <select
                id="booking-service"
                class="w-full px-4 py-3 rounded-xl bg-zinc-900/90 border border-white/15 text-white focus:outline-none focus:border-amber-400"
              ></select>
            </div>
            <div>
              <label for="booking-vehicle" class="block text-xs font-bold uppercase tracking-wider text-zinc-300 mb-2">Vehicle Size</label>
              <select
                id="booking-vehicle"
                class="w-full px-4 py-3 rounded-xl bg-zinc-900/90 border border-white/15 text-white focus:outline-none focus:border-amber-400"
              >
                <option value="sedan">Coupe / Sedan (Base)</option>
                <option value="suv">Mid-Size / 2-Row SUV (+$25)</option>
                <option value="truck">Truck / 3-Row SUV (+$50)</option>
              </select>
            </div>
          </div>

          <div class="grid sm:grid-cols-2 gap-5">
            <div>
              <label for="preferred-date" class="block text-xs font-bold uppercase tracking-wider text-zinc-300 mb-2">Preferred Date</label>
              <input
                id="preferred-date"
                type="date"
                class="w-full px-4 py-3 rounded-xl bg-zinc-900/90 border border-white/15 text-white focus:outline-none focus:border-amber-400"
              />
            </div>
            <div>
              <label for="service-address" class="block text-xs font-bold uppercase tracking-wider text-zinc-300 mb-2">Home or Work Location</label>
              <input
                id="service-address"
                type="text"
                placeholder="Street address or neighborhood"
                class="w-full px-4 py-3 rounded-xl bg-zinc-900/90 border border-white/15 text-white placeholder-zinc-500 focus:outline-none focus:border-amber-400"
              />
            </div>
          </div>

          <!-- Optional Add-On Checkbox -->
          <div class="p-4 rounded-2xl bg-amber-500/10 border border-amber-400/25">
            <label class="flex items-start gap-3 cursor-pointer">
              <input
                id="addon-headlights"
                type="checkbox"
                class="mt-1 w-4 h-4 rounded accent-amber-500"
              />
              <span class="text-sm text-zinc-200">
                <span class="font-bold text-amber-300">Add Headlight Restoration (+$60 • +1 Hr)</span>
                <span class="block text-xs text-zinc-400 mt-0.5">Includes oxidation &amp; haze removal plus protective coating to help slow future fading.</span>
              </span>
            </label>
          </div>

          <div>
            <label for="vehicle-notes" class="block text-xs font-bold uppercase tracking-wider text-zinc-300 mb-2">Vehicle &amp; Condition Notes</label>
            <textarea
              id="vehicle-notes"
              rows="3"
              placeholder="Year, make, model, stains, pet hair, or questions..."
              class="w-full px-4 py-3 rounded-xl bg-zinc-900/90 border border-white/15 text-white placeholder-zinc-500 focus:outline-none focus:border-amber-400"
            ></textarea>
          </div>

          <button
            type="submit"
            class="w-full py-4 px-6 rounded-2xl font-bold text-base text-black transition-all transform hover:-translate-y-0.5"
            style="background: linear-gradient(135deg, #fde047 0%, var(--accent-primary) 55%, var(--sunset-secondary) 100%); box-shadow: 0 10px 28px var(--accent-glow);"
          >
            Review &amp; Request Booking
          </button>
        </form>

        <!-- Live Estimate Summary Card -->
        <aside class="lg:col-span-5 metallic-card rounded-3xl p-6 sm:p-8 space-y-6">
          <div class="flex items-center justify-between border-b border-white/10 pb-4">
            <div>
              <span class="text-xs font-bold uppercase tracking-wider text-amber-400">Live Summary</span>
              <h3 class="font-display text-2xl font-extrabold text-white mt-0.5">Estimated Quote</h3>
            </div>
            <span class="px-3 py-1 rounded-full text-xs font-bold bg-amber-500/15 text-amber-300 border border-amber-400/30">
              We Come To You!
            </span>
          </div>

          <div class="space-y-3 text-sm">
            <div class="flex justify-between text-zinc-300">
              <span>Selected Service</span>
              <span id="summary-service-name" class="font-semibold text-white">Full In &amp; Out Detail</span>
            </div>
            <div class="flex justify-between text-zinc-300">
              <span>Vehicle Size</span>
              <span id="summary-vehicle-name" class="font-semibold text-white">Coupe / Sedan</span>
            </div>
            <div class="flex justify-between text-zinc-300">
              <span>Headlight Add-On</span>
              <span id="summary-addon-status" class="font-semibold text-zinc-400">Not included</span>
            </div>
            <div class="flex justify-between text-zinc-300">
              <span>Estimated Time</span>
              <span id="summary-duration" class="font-bold text-amber-300">6 Hours</span>
            </div>
          </div>

          <div class="p-5 rounded-2xl bg-zinc-900/90 border border-amber-400/25">
            <div class="text-xs font-semibold uppercase tracking-wider text-zinc-400">Estimated Total</div>
            <div id="summary-price" class="font-display text-3xl sm:text-4xl font-extrabold text-gold-gradient mt-1">$200</div>
            <p id="summary-note" class="text-xs text-zinc-400 mt-2">
              Final price confirmed upon arrival based on overall vehicle condition.
            </p>
          </div>

          <div class="text-xs text-zinc-400 space-y-2 pt-2 border-t border-white/10">
            <p class="font-semibold text-zinc-200">Need a custom quote or quick question?</p>
            <p>Call or text KustomDetailz directly at <a href="tel:+17124908490" class="text-amber-300 font-bold hover:underline">(712) 490-8490</a>.</p>
          </div>
        </aside>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="border-t border-white/10 bg-zinc-950 py-12">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col sm:flex-row items-center justify-between gap-6">
      <div class="flex items-center gap-3">
        <div class="h-11 w-20 rounded-xl overflow-hidden border border-amber-400/35 bg-black flex items-center justify-center shrink-0">
          <img
            data-logo-img
            src="./image_1277c7.jpg"
            alt="KustomDetailz Logo"
            onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
            class="w-full h-full object-cover"
          />
          <div class="hidden w-full h-full items-center justify-center text-amber-400 font-display font-extrabold text-xs tracking-wider">KD</div>
        </div>
        <div>
          <p class="font-display font-extrabold text-lg leading-none">
            <span class="text-chrome-gradient">Kustom</span><span class="text-gold-gradient">Detailz</span>
          </p>
          <p class="text-[11px] font-bold tracking-widest text-amber-400/90 uppercase mt-1">
            DETAIL • PROTECT • SHINE • WE COME TO YOU!
          </p>
        </div>
      </div>

      <div class="text-center sm:text-right text-sm text-zinc-400 space-y-1">
        <p>
          Phone: <a href="tel:+17124908490" class="text-amber-300 font-semibold hover:underline">(712) 490-8490</a>
        </p>
        <p class="text-xs text-zinc-500">&copy; <span id="current-year"></span> KustomDetailz. All rights reserved.</p>
      </div>
    </div>
  </footer>

  <!-- SERVICE FULL CHECKLIST MODAL -->
  <div id="checklist-modal" class="fixed inset-0 z-50 hidden items-center justify-center p-4 bg-black/80 backdrop-blur-sm">
    <div class="metallic-card max-w-2xl w-full max-h-[88vh] overflow-y-auto rounded-3xl p-6 sm:p-8 border border-amber-400/30 relative">
      <div class="flex items-start justify-between gap-4 border-b border-white/10 pb-4 mb-5">
        <div>
          <span id="modal-badge" class="inline-block text-[11px] font-bold uppercase tracking-wider px-2.5 py-1 rounded-full bg-amber-500/15 text-amber-300 border border-amber-400/30 mb-2">
            We Come To You!
          </span>
          <h3 id="modal-title" class="font-display text-2xl sm:text-3xl font-extrabold text-white"></h3>
          <p id="modal-tagline" class="text-sm font-medium text-amber-300 mt-1"></p>
        </div>
        <button
          id="close-modal-btn"
          type="button"
          aria-label="Close checklist modal"
          class="p-2 rounded-xl text-zinc-400 hover:text-white hover:bg-white/10 transition-colors"
        >
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
      </div>

      <div class="grid grid-cols-2 sm:grid-cols-3 gap-3 mb-6 text-sm">
        <div class="p-3 rounded-2xl bg-zinc-900/90 border border-white/10">
          <div class="text-xs text-zinc-400">Estimated Time</div>
          <div id="modal-duration" class="font-bold text-white mt-0.5"></div>
        </div>
        <div class="p-3 rounded-2xl bg-zinc-900/90 border border-white/10">
          <div class="text-xs text-zinc-400">Pricing</div>
          <div id="modal-price" class="font-bold text-amber-300 mt-0.5"></div>
        </div>
        <div class="col-span-2 sm:col-span-1 p-3 rounded-2xl bg-zinc-900/90 border border-white/10">
          <div class="text-xs text-zinc-400">Location</div>
          <div class="font-bold text-white mt-0.5">We Come To You!</div>
        </div>
      </div>

      <div class="space-y-4 text-sm text-zinc-300 leading-relaxed">
        <div>
          <h4 class="font-display font-bold text-white text-base mb-1.5">Service Description</h4>
          <p id="modal-description"></p>
        </div>

        <div id="modal-sections" class="space-y-4 pt-2"></div>

        <p id="modal-closing" class="pt-3 border-t border-white/10 text-amber-200/90 font-medium"></p>
      </div>

      <div class="mt-7 pt-4 border-t border-white/10 flex flex-col sm:flex-row gap-3 justify-end">
        <button
          id="modal-select-btn"
          type="button"
          class="px-6 py-3 rounded-xl font-bold text-sm text-black"
          style="background: linear-gradient(135deg, #fde047 0%, var(--accent-primary) 60%, var(--sunset-secondary) 100%);"
        >
          Select Service in Estimator
        </button>
      </div>
    </div>
  </div>

  <!-- BOOKING SUMMARY MODAL (No alert() or confirm() used) -->
  <div id="booking-modal" class="fixed inset-0 z-50 hidden items-center justify-center p-4 bg-black/80 backdrop-blur-sm">
    <div class="metallic-card max-w-lg w-full rounded-3xl p-6 sm:p-8 border border-amber-400/35 space-y-5">
      <div class="flex items-center justify-between border-b border-white/10 pb-3">
        <h3 class="font-display text-2xl font-extrabold text-white">Booking Request Ready</h3>
        <button
          id="close-booking-modal-btn"
          type="button"
          aria-label="Close booking summary"
          class="p-2 rounded-xl text-zinc-400 hover:text-white hover:bg-white/10"
        >
          <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
      </div>

      <p class="text-sm text-zinc-300 leading-relaxed">
        Here is your summary for <strong class="text-amber-300">KustomDetailz</strong>. Call or text <a href="tel:+17124908490" class="text-amber-300 font-bold underline">(712) 490-8490</a> to lock in your mobile appointment time.
      </p>

      <div id="booking-summary-details" class="p-4 rounded-2xl bg-zinc-900/90 border border-white/10 text-sm space-y-2 text-zinc-200"></div>

      <div class="flex flex-col sm:flex-row gap-3 pt-2">
        <a
          href="tel:+17124908490"
          class="flex-1 text-center py-3 px-4 rounded-xl font-bold text-sm text-black"
          style="background: linear-gradient(135deg, #fde047 0%, var(--accent-primary) 60%, var(--sunset-secondary) 100%);"
        >
          Call (712) 490-8490
        </a>
        <button
          id="done-booking-modal-btn"
          type="button"
          class="py-3 px-5 rounded-xl font-semibold text-sm text-zinc-200 bg-white/10 hover:bg-white/15"
        >
          Done
        </button>
      </div>
    </div>
  </div>

  <!-- SITE CONFIGURATION & INTERACTIVE LOGIC -->
  <script>
    const SITE_CONFIG = {
      businessName: "KustomDetailz",
      motto: "DETAIL • PROTECT • SHINE",
      phoneDisplay: "(712) 490-8490",
      phoneHref: "tel:+17124908490",
      locationLabel: "We Come To You!",
      logoImageUrl: "./image_1277c7.jpg",
      vehicleUpcharges: {
        sedan: { label: "Coupe / Sedan", addPrice: 0 },
        suv: { label: "Mid-Size / 2-Row SUV", addPrice: 25 },
        truck: { label: "Truck / 3-Row SUV", addPrice: 50 }
      },
      services: [
        {
          id: "full-detail",
          name: "Full In & Out Detail",
          badge: "Best Value",
          tagline: "A Complete Interior & Exterior Transformation",
          duration: "6 Hours",
          durationHours: 6,
          basePrice: 200,
          priceDisplayPrefix: "Starting At",
          isCustomQuote: false,
          location: "We Come To You!",
          description: "Our Full Detail package is designed to give your vehicle a complete refresh from top to bottom. We take pride in the little things, using quality, vehicle-safe products and professional detailing techniques to bring out the best in your ride. Whether you're looking to freshen up your daily driver or bring some extra shine back to your vehicle, we put care and attention into every detail.",
          checklistSections: [
            {
              heading: "Exterior Detail Includes",
              items: [
                "Thorough hand wash using premium, paint-safe products.",
                "Deep cleaning of wheels, tires, and wheel wells.",
                "Removal of bugs, tar, and everyday road buildup.",
                "Detailed cleaning of door jambs and exterior entry areas.",
                "Professional tire dressing for a clean, rich finish.",
                "Final exterior wipe-down for a smooth, spotless appearance."
              ]
            },
            {
              heading: "Interior Detail Includes",
              items: [
                "Complete vacuuming of carpets, seats, and trunk area.",
                "Detailed cleaning of interior surfaces and panels.",
                "Deep cleaning of cup holders, air vents, and hard-to-reach crevices.",
                "Thorough cleaning of interior windows and mirrors for a streak-free finish.",
                "Light interior deodorizing to leave your vehicle feeling fresh and clean."
              ]
            }
          ],
          closing: "At KustomDetailz, it's all in the details. We don't just clean your ride — we bring back the pride in driving it!"
        },
        {
          id: "interior-detail",
          name: "Interior Detail",
          badge: "Cabin Refresh",
          tagline: "Refresh Your Ride. Restore That Fresh Interior Feel.",
          duration: "4 Hours",
          durationHours: 4,
          basePrice: 150,
          priceDisplayPrefix: "Starting At",
          isCustomQuote: false,
          location: "We Come To You!",
          description: "Our Interior Detail is designed to bring your vehicle's cabin back to a clean, refreshed, and well-maintained condition. We focus on the areas you see and touch every day, removing everyday dirt, dust, and buildup while giving your interior the attention it deserves. From carpets and seats to those hard-to-reach cracks and crevices, we take pride in the little details that make a big difference.",
          checklistSections: [
            {
              heading: "Interior Detail Includes",
              items: [
                "Thorough vacuuming of carpets, seats, and floor mats.",
                "Detailed cleaning and wipe-down of interior surfaces.",
                "Cleaning of door panels, cup holders, and interior trim.",
                "Attention to hard-to-reach areas and everyday buildup.",
                "Light stain treatment where possible.",
                "Interior glass and mirrors cleaned for a clear, streak-free finish.",
                "Interior surfaces left clean, refreshed, and protected."
              ]
            }
          ],
          closing: "At KustomDetailz, we believe your vehicle should feel just as good on the inside as it looks on the outside. It's all in the details!"
        },
        {
          id: "exterior-detail",
          name: "Exterior Detail",
          badge: "Gloss & Seal",
          tagline: "Bring Back the Shine. Protect Your Investment.",
          duration: "3 Hours",
          durationHours: 3,
          basePrice: 75,
          priceDisplayPrefix: "Starting At",
          isCustomQuote: false,
          location: "We Come To You!",
          description: "Our Exterior Detail is designed to restore your vehicle's shine while removing everyday dirt, grime, and buildup. We use premium, paint-safe products and careful detailing techniques to leave your vehicle looking refreshed, glossy, and well-maintained. From the wheels to the paint, we pay attention to every detail to give your ride the clean finish it deserves.",
          checklistSections: [
            {
              heading: "Exterior Detail Includes",
              items: [
                "Thorough hand wash using premium, paint-safe products.",
                "Gentle hand drying to help minimize the risk of swirl marks and scratches.",
                "Detailed cleaning of wheels, tires, and wheel wells to remove brake dust, dirt, and road grime.",
                "Removal of light tar, tree sap, and bug residue from exterior paint.",
                "Detailed cleaning of door jambs and fuel door areas.",
                "Exterior trim cleaning and dressing for a refreshed appearance.",
                "Premium paint sealant application for enhanced gloss and short-term protection against the elements.",
                "Exterior glass cleaning for a clear, streak-free finish.",
                "Final inspection and finishing touches to ensure your vehicle looks its best."
              ]
            }
          ],
          closing: "At KustomDetailz, we believe a clean exterior is more than just a shine — it's about protecting your investment and taking pride in your ride!"
        },
        {
          id: "paint-polishing",
          name: "Paint Polishing",
          badge: "Single-Step Polish",
          tagline: "Restore the Gloss. Refine the Finish. Bring Your Paint Back to Life.",
          duration: "6 Hours",
          durationHours: 6,
          basePrice: null,
          priceDisplayPrefix: "Pricing",
          isCustomQuote: true,
          location: "We Come To You!",
          description: "Our Paint Polishing service is designed to enhance your vehicle's appearance by restoring gloss, improving paint clarity, and reducing the look of light surface imperfections. Over time, everyday driving, environmental exposure, and improper washing can leave your paint looking dull, faded, and lacking its original shine. We take the time to properly prepare your vehicle's exterior before performing a professional single-step machine polish to bring out a smoother, more vibrant finish. We complete the service with a durable paint sealant to help protect your paint and maintain that freshly detailed look.",
          checklistSections: [
            {
              heading: "Paint Polishing Includes",
              items: [
                "Thorough hand wash using premium, paint-safe products.",
                "Detailed cleaning of wheels and tires.",
                "Paint decontamination to remove embedded dirt, tar, tree sap, and bug residue.",
                "Single-step machine polishing to enhance gloss and clarity.",
                "Reduction of light paint imperfections and surface blemishes.",
                "Application of a durable paint sealant for added shine and protection.",
                "Professional tire dressing for a clean, finished appearance.",
                "Final inspection to ensure your vehicle leaves with a refreshed, glossy finish."
              ]
            }
          ],
          closing: "At KustomDetailz, we believe your paint deserves more than just a wash. We bring back the gloss, enhance the finish, and make your ride stand out wherever it goes!"
        },
        {
          id: "headlight-restoration",
          name: "Headlight Restoration",
          badge: "Night Visibility",
          tagline: "Restore Clarity. Bring Back the Shine. Improve Your Visibility.",
          duration: "1 Hour",
          durationHours: 1,
          basePrice: 60,
          priceDisplayPrefix: "Price",
          isCustomQuote: false,
          location: "We Come To You!",
          description: "Cloudy, faded headlights? Let us bring them back to life with our professional Headlight Restoration service! Our Headlight Restoration service is designed to restore the clarity and appearance of dull, cloudy, and oxidized headlights. Over time, exposure to the sun and elements can cause headlights to fade, reducing their brightness and affecting nighttime visibility. We use safe restoration techniques to remove oxidation and surface haze, helping bring your headlights back to a cleaner, clearer appearance. To finish the service, we apply a protective coating to help slow down future fading and keep your headlights looking their best.",
          checklistSections: [
            {
              heading: "Headlight Restoration Includes",
              items: [
                "Thorough cleaning and preparation of headlight lenses.",
                "Removal of oxidation, cloudiness, and surface haze.",
                "Professional restoration to improve headlight clarity.",
                "Refinishing for a brighter, refreshed appearance.",
                "Application of a protective coating to help slow future fading.",
                "Final inspection to ensure a clean, clear finish."
              ]
            }
          ],
          closing: "At KustomDetailz, the little details make a big difference. Restore your headlights, refresh your ride, and see the road ahead with confidence!"
        }
      ]
    };

    const state = {
      selectedVehicle: "sedan",
      selectedServiceId: "full-detail",
      addonHeadlights: false,
      activeModalServiceId: null
    };

    function formatPriceForService(service, vehicleKey) {
      if (service.isCustomQuote || service.basePrice === null) {
        return `Call for a Custom Quote (${SITE_CONFIG.phoneDisplay})`;
      }
      const upcharge = SITE_CONFIG.vehicleUpcharges[vehicleKey]?.addPrice || 0;
      const total = service.basePrice + upcharge;
      return `${service.priceDisplayPrefix}: $${total}`;
    }

    function renderServicesGrid() {
      const grid = document.getElementById("services-grid");
      if (!grid) return;

      grid.innerHTML = SITE_CONFIG.services.map((service) => {
        const isFeatured = service.id === "full-detail";
        const priceLabel = formatPriceForService(service, state.selectedVehicle);
        const primaryBullets = service.checklistSections[0]?.items.slice(0, 4) || [];

        return `
          <article class="metallic-card rounded-3xl p-6 flex flex-col justify-between transition-all ${isFeatured ? "ring-2 ring-amber-400/50" : ""}">
            <div>
              <div class="flex items-center justify-between gap-2 mb-4">
                <span class="px-3 py-1 rounded-full text-xs font-bold uppercase tracking-wider bg-amber-500/15 text-amber-300 border border-amber-400/30">
                  ${service.badge}
                </span>
                <span class="text-xs font-semibold text-zinc-400">${service.location}</span>
              </div>

              <h3 class="font-display text-2xl font-extrabold text-white">${service.name}</h3>
              <p class="text-xs font-medium text-amber-300/90 mt-1">${service.tagline}</p>

              <div class="mt-4 pt-4 border-t border-white/10 flex flex-wrap items-baseline justify-between gap-2">
                <span class="font-display text-lg font-extrabold text-white">${priceLabel}</span>
                <span class="text-xs font-semibold text-zinc-400">Est. Time: ${service.duration}</span>
              </div>

              <p class="text-sm text-zinc-400 mt-3 line-clamp-3 leading-relaxed">
                ${service.description}
              </p>

              <ul class="mt-4 space-y-2 text-xs sm:text-sm text-zinc-300">
                ${primaryBullets.map((item) => `
                  <li class="flex items-start gap-2">
                    <span class="text-amber-400 font-bold mt-0.5">✓</span>
                    <span>${item}</span>
                  </li>
                `).join("")}
              </ul>
            </div>

            <div class="mt-6 pt-4 border-t border-white/10 flex flex-col sm:flex-row gap-2.5">
              <button
                type="button"
                onclick="openChecklistModal('${service.id}')"
                class="flex-1 py-2.5 px-4 rounded-xl text-xs sm:text-sm font-semibold text-amber-200 bg-white/5 hover:bg-white/10 border border-white/15 transition-colors"
              >
                View Full Checklist
              </button>
              <button
                type="button"
                onclick="chooseServiceForBooking('${service.id}')"
                class="flex-1 py-2.5 px-4 rounded-xl text-xs sm:text-sm font-bold text-black transition-transform hover:-translate-y-0.5"
                style="background: linear-gradient(135deg, #fde047 0%, var(--accent-primary) 60%, var(--sunset-secondary) 100%);"
              >
                Select Service
              </button>
            </div>
          </article>
        `;
      }).join("");

      updateVehicleButtonsUI();
    }

    function updateVehicleButtonsUI() {
      document.querySelectorAll(".vehicle-btn").forEach((btn) => {
        const isActive = btn.dataset.size === state.selectedVehicle;
        btn.className = isActive
          ? "vehicle-btn px-4 py-2.5 rounded-xl text-sm font-bold text-black transition-all shadow"
          : "vehicle-btn px-4 py-2.5 rounded-xl text-sm font-semibold text-zinc-300 hover:text-white transition-all";
        if (isActive) {
          btn.style.background = "linear-gradient(135deg, #fde047 0%, var(--accent-primary) 60%, var(--sunset-secondary) 100%)";
        } else {
          btn.style.background = "transparent";
        }
      });
    }

    function populateBookingSelect() {
      const select = document.getElementById("booking-service");
      if (!select) return;
      select.innerHTML = SITE_CONFIG.services.map((s) => {
        const label = s.isCustomQuote
          ? `${s.name} (${s.duration} • Custom Quote)`
          : `${s.name} (${s.duration} • From $${s.basePrice})`;
        return `<option value="${s.id}">${label}</option>`;
      }).join("");
      select.value = state.selectedServiceId;
    }

    function updateBookingEstimate() {
      const service = SITE_CONFIG.services.find((s) => s.id === state.selectedServiceId) || SITE_CONFIG.services[0];
      const vehicle = SITE_CONFIG.vehicleUpcharges[state.selectedVehicle] || SITE_CONFIG.vehicleUpcharges.sedan;
      const addonCost = state.addonHeadlights ? 60 : 0;
      const addonHours = state.addonHeadlights ? 1 : 0;
      const totalHours = service.durationHours + addonHours;

      document.getElementById("summary-service-name").textContent = service.name;
      document.getElementById("summary-vehicle-name").textContent = vehicle.label;
      document.getElementById("summary-addon-status").textContent = state.addonHeadlights ? "+$60 • +1 Hr" : "Not included";
      document.getElementById("summary-duration").textContent = `${totalHours} ${totalHours === 1 ? "Hour" : "Hours"}`;

      const priceEl = document.getElementById("summary-price");
      const noteEl = document.getElementById("summary-note");

      if (service.isCustomQuote || service.basePrice === null) {
        priceEl.textContent = "Custom Quote";
        noteEl.textContent = `Paint Polishing is quoted by vehicle & paint condition. Call or text ${SITE_CONFIG.phoneDisplay} for a custom quote${addonCost > 0 ? " (+$60 Headlight Restoration add-on)" : ""}.`;
      } else {
        const total = service.basePrice + vehicle.addPrice + addonCost;
        priceEl.textContent = `$${total}`;
        noteEl.textContent = "Estimated total based on selected service, vehicle size, and add-ons. Final price confirmed upon arrival.";
      }
    }

    function openChecklistModal(serviceId) {
      const service = SITE_CONFIG.services.find((s) => s.id === serviceId);
      if (!service) return;
      state.activeModalServiceId = serviceId;

      document.getElementById("modal-badge").textContent = `${service.badge} • ${service.location}`;
      document.getElementById("modal-title").textContent = service.name;
      document.getElementById("modal-tagline").textContent = service.tagline;
      document.getElementById("modal-duration").textContent = service.duration;
      document.getElementById("modal-price").textContent = formatPriceForService(service, state.selectedVehicle);
      document.getElementById("modal-description").textContent = service.description;
      document.getElementById("modal-closing").textContent = service.closing;

      document.getElementById("modal-sections").innerHTML = service.checklistSections.map((sec) => `
        <div>
          <h4 class="font-display font-bold text-white text-base mb-2">${sec.heading}</h4>
          <ul class="space-y-2 text-sm text-zinc-300">
            ${sec.items.map((line) => `
              <li class="flex items-start gap-2.5">
                <span class="text-amber-400 font-bold mt-0.5">•</span>
                <span>${line}</span>
              </li>
            `).join("")}
          </ul>
        </div>
      `).join("");

      const modal = document.getElementById("checklist-modal");
      modal.classList.remove("hidden");
      modal.classList.add("flex");
    }

    function closeChecklistModal() {
      const modal = document.getElementById("checklist-modal");
      modal.classList.add("hidden");
      modal.classList.remove("flex");
    }

    function chooseServiceForBooking(serviceId) {
      state.selectedServiceId = serviceId;
      const select = document.getElementById("booking-service");
      if (select) select.value = serviceId;
      updateBookingEstimate();
      closeChecklistModal();
      document.getElementById("booking")?.scrollIntoView({ behavior: "smooth" });
    }

    function initEvents() {
      // Set current copyright year
      const yearEl = document.getElementById("current-year");
      if (yearEl) yearEl.textContent = new Date().getFullYear();

      // Apply configured logo image path safely with fallback kept intact
      if (SITE_CONFIG.logoImageUrl && SITE_CONFIG.logoImageUrl.trim() !== "") {
        document.querySelectorAll("[data-logo-img]").forEach((img) => {
          img.src = SITE_CONFIG.logoImageUrl.trim();
        });
      }

      // Mobile nav toggle
      const menuBtn = document.getElementById("mobile-menu-btn");
      const mobileMenu = document.getElementById("mobile-menu");
      const iconOpen = document.getElementById("menu-icon-open");
      const iconClose = document.getElementById("menu-icon-close");

      menuBtn?.addEventListener("click", () => {
        const isOpen = !mobileMenu.classList.contains("hidden");
        mobileMenu.classList.toggle("hidden", isOpen);
        iconOpen.classList.toggle("hidden", !isOpen);
        iconClose.classList.toggle("hidden", isOpen);
      });

      document.querySelectorAll(".mobile-nav-link").forEach((link) => {
        link.addEventListener("click", () => {
          mobileMenu.classList.add("hidden");
          iconOpen.classList.remove("hidden");
          iconClose.classList.add("hidden");
        });
      });

      // Vehicle size buttons
      document.querySelectorAll(".vehicle-btn").forEach((btn) => {
        btn.addEventListener("click", () => {
          state.selectedVehicle = btn.dataset.size;
          const bookingVehicleSelect = document.getElementById("booking-vehicle");
          if (bookingVehicleSelect) bookingVehicleSelect.value = state.selectedVehicle;
          renderServicesGrid();
          updateBookingEstimate();
        });
      });

      // Before / After slider
      const rangeInput = document.getElementById("comparison-range");
      const beforeLayer = document.getElementById("before-layer");
      const divider = document.getElementById("comparison-divider");
      rangeInput?.addEventListener("input", (e) => {
        const val = Number(e.target.value);
        const rightClip = 100 - val;
        beforeLayer.style.clipPath = `inset(0 ${rightClip}% 0 0)`;
        divider.style.left = `${val}%`;
      });

      // Booking form controls
      document.getElementById("booking-service")?.addEventListener("change", (e) => {
        state.selectedServiceId = e.target.value;
        updateBookingEstimate();
      });

      document.getElementById("booking-vehicle")?.addEventListener("change", (e) => {
        state.selectedVehicle = e.target.value;
        renderServicesGrid();
        updateBookingEstimate();
      });

      document.getElementById("addon-headlights")?.addEventListener("change", (e) => {
        state.addonHeadlights = e.target.checked;
        updateBookingEstimate();
      });

      // Checklist modal controls
      document.getElementById("close-modal-btn")?.addEventListener("click", closeChecklistModal);
      document.getElementById("checklist-modal")?.addEventListener("click", (e) => {
        if (e.target.id === "checklist-modal") closeChecklistModal();
      });
      document.getElementById("modal-select-btn")?.addEventListener("click", () => {
        if (state.activeModalServiceId) {
          chooseServiceForBooking(state.activeModalServiceId);
        }
      });

      // Booking form submit -> interactive modal summary
      const bookingForm = document.getElementById("booking-form");
      const bookingModal = document.getElementById("booking-modal");
      const summaryDetails = document.getElementById("booking-summary-details");

      bookingForm?.addEventListener("submit", (e) => {
        e.preventDefault();
        const name = document.getElementById("customer-name").value.trim();
        const phone = document.getElementById("customer-phone").value.trim();
        const dateVal = document.getElementById("preferred-date").value || "Flexible / Soonest Available";
        const addressVal = document.getElementById("service-address").value.trim() || "We Come To You (Location TBD)";
        const notesVal = document.getElementById("vehicle-notes").value.trim();

        const service = SITE_CONFIG.services.find((s) => s.id === state.selectedServiceId) || SITE_CONFIG.services[0];
        const vehicle = SITE_CONFIG.vehicleUpcharges[state.selectedVehicle] || SITE_CONFIG.vehicleUpcharges.sedan;
        const addonCost = state.addonHeadlights ? 60 : 0;
        const addonHours = state.addonHeadlights ? 1 : 0;
        const totalHours = service.durationHours + addonHours;
        const estimateText = (service.isCustomQuote || service.basePrice === null)
          ? "Custom Quote"
          : `$${service.basePrice + vehicle.addPrice + addonCost}`;

        summaryDetails.innerHTML = `
          <div><span class="text-zinc-400">Name:</span> <strong class="text-white">${name}</strong></div>
          <div><span class="text-zinc-400">Customer Phone:</span> <strong class="text-white">${phone}</strong></div>
          <div><span class="text-zinc-400">Service:</span> <strong class="text-amber-300">${service.name}</strong></div>
          <div><span class="text-zinc-400">Vehicle Size:</span> <strong class="text-white">${vehicle.label}</strong></div>
          <div><span class="text-zinc-400">Headlight Add-On:</span> <strong class="text-white">${state.addonHeadlights ? "Yes (+$60 • +1 Hr)" : "No"}</strong></div>
          <div><span class="text-zinc-400">Estimated Time &amp; Price:</span> <strong class="text-amber-300">${totalHours} Hrs • ${estimateText}</strong></div>
          <div><span class="text-zinc-400">Preferred Date:</span> <strong class="text-white">${dateVal}</strong></div>
          <div><span class="text-zinc-400">Location:</span> <strong class="text-white">${addressVal}</strong></div>
          ${notesVal ? `<div><span class="text-zinc-400">Notes:</span> <span class="text-zinc-200">${notesVal}</span></div>` : ""}
        `;

        bookingModal.classList.remove("hidden");
        bookingModal.classList.add("flex");
      });

      const hideBookingModal = () => {
        bookingModal.classList.add("hidden");
        bookingModal.classList.remove("flex");
      };

      document.getElementById("close-booking-modal-btn")?.addEventListener("click", hideBookingModal);
      document.getElementById("done-booking-modal-btn")?.addEventListener("click", hideBookingModal);
      bookingModal?.addEventListener("click", (e) => {
        if (e.target.id === "booking-modal") hideBookingModal();
      });
    }

    document.addEventListener("DOMContentLoaded", () => {
      renderServicesGrid();
      populateBookingSelect();
      updateBookingEstimate();
      initEvents();
    });
  </script>
</body>
</html>