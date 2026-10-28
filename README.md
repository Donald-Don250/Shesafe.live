<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>SheSafe Live - Know if a street is safe BEFORE you walk it</title>
    <meta
      name="description"
      content="AI-powered safety insights and real women reporting live. Know if a street is safe before you walk it."
    />
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <style>
      body {
        font-family: 'Inter', sans-serif;
      }
      .soft-shadow {
        box-shadow: 0 18px 50px rgba(26, 43, 92, 0.12);
      }
      .section-shell {
        max-width: 1200px;
        margin: 0 auto;
      }
    </style>
  </head>
  <body class="bg-white text-slate-900 antialiased">
    <div class="bg-[#1A2B5C] text-white">
      <div class="section-shell flex items-center justify-center gap-2 px-6 py-2.5 text-sm md:text-xs">
        <span class="inline-block h-2.5 w-2.5 rounded-full bg-green-400 animate-pulse"></span>
        <span class="font-bold">LIVE:</span>
        <span>Protecting women in 190+ countries • Works offline • Encrypted</span>
      </div>
    </div>

    <header class="sticky top-0 z-50 border-b border-slate-100 bg-white/95 backdrop-blur-sm">
      <div class="section-shell flex items-center justify-between px-6 py-4 md:px-12">
        <div class="flex items-center gap-3">
          <div class="flex h-9 w-9 items-center justify-center rounded-xl bg-blue-100 text-xl">🛡️</div>
          <h1 class="text-xl font-black text-[#1A2B5C] md:text-2xl">SheSafe Live</h1>
        </div>

        <nav class="hidden items-center gap-8 text-sm font-medium text-[#1A2B5C] md:flex">
          <a href="#how-it-works" class="transition hover:text-blue-600">How it works</a>
          <a href="#safety-map" class="transition hover:text-blue-600">Safety Map</a>
          <a href="#pricing" class="transition hover:text-blue-600">Pricing</a>
        </nav>

        <a
          href="#pricing"
          class="rounded-lg bg-[#1A2B5C] px-5 py-2.5 text-sm font-bold text-white transition hover:bg-[#233a75]"
        >
          Open App
        </a>
      </div>
    </header>

    <main>
      <section class="bg-white px-6 py-12 md:px-12 md:py-20">
        <div class="section-shell grid items-center gap-12 md:grid-cols-2">
          <div>
            <h2 class="max-w-xl text-5xl font-black leading-[0.95] tracking-tight text-[#1A2B5C] md:text-6xl">
              Know if a street is safe<br />BEFORE you walk it
            </h2>
            <p class="mt-6 max-w-xl text-lg leading-relaxed text-slate-600">
              AI-powered safety insights + real women reporting live. For solo walks, night shifts,
              and new cities.
            </p>

            <div class="mt-8 max-w-lg">
              <div class="flex flex-col gap-3 sm:flex-row">
                <div class="flex flex-1 items-center rounded-full border border-blue-200 bg-blue-50/60 px-4 py-3">
                  <span class="mr-2 text-lg">📍</span>
                  <input
                    id="cityInput"
                    type="text"
                    placeholder="Your city: London, São Paulo, Tokyo"
                    class="w-full border-none bg-transparent text-sm text-slate-700 outline-none placeholder:text-slate-400"
                    aria-label="City"
                  />
                </div>
                <button
                  type="button"
                  id="checkSafetyBtn"
                  class="rounded-full bg-[#1A2B5C] px-6 py-3 text-sm font-bold text-white transition hover:bg-[#233a75]"
                >
                  🛡️ Check Safety
                </button>
              </div>
              <p class="mt-3 text-sm text-slate-500">Enterprise-grade security • We never sell your location</p>
            </div>

            <div id="resultBox" class="mt-6 hidden max-w-lg rounded-2xl border border-green-200 bg-green-50 p-4" aria-live="polite">
              <p class="text-xs font-bold uppercase tracking-wide text-green-700">Safe • Low risk • Demo</p>
              <p id="resultTitle" class="mt-1 text-xl font-black text-slate-900">87/100 Safe - Well-lit, high foot traffic</p>
              <p id="resultQuote" class="mt-1 text-xs text-slate-500">"Saved me on my night shift" - Sarah, London</p>
            </div>
          </div>

          <div class="flex justify-center">
            <div class="soft-shadow h-[550px] w-[300px] rounded-[30px] border-[8px] border-black bg-[#1A2B5C] p-3">
              <div class="relative h-full overflow-hidden rounded-[22px] bg-[#E0E6F0]">
                <div class="m-3 rounded-xl bg-white p-3 shadow-sm">
                  <p class="inline-block rounded-md bg-[#1A2B5C] px-2 py-1 text-xs font-bold text-white">
                    Live Map • 190+ countries
                  </p>
                </div>

                <div class="absolute inset-0 bg-[radial-gradient(circle_at_center,_rgba(59,130,246,0.15),_transparent_55%)]"></div>
                <div class="absolute inset-x-4 top-16">
                  <div class="flex justify-between text-[10px] font-semibold text-slate-500">
                    <span>Low risk</span>
                    <span>0.8 mi</span>
                  </div>
                  <div class="mt-3 h-32 rounded-2xl bg-white/80 p-3 shadow-sm backdrop-blur-sm">
                    <div class="flex h-full items-end justify-between gap-2">
                      <div class="w-full rounded-t-xl bg-emerald-300" style="height: 55%"></div>
                      <div class="w-full rounded-t-xl bg-yellow-300" style="height: 70%"></div>
                      <div class="w-full rounded-t-xl bg-orange-300" style="height: 85%"></div>
                      <div class="w-full rounded-t-xl bg-rose-300" style="height: 35%"></div>
                    </div>
                  </div>
                </div>

                <div class="absolute inset-x-4 bottom-4">
                  <button type="button" class="w-full rounded-xl bg-[#1A2B5C] py-3 text-sm font-bold text-white">
                    Start Live Share
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <section id="how-it-works" class="bg-slate-50 px-6 py-16 md:px-12">
        <div class="section-shell">
          <div class="mx-auto max-w-2xl text-center">
            <p class="text-sm font-bold uppercase tracking-[0.2em] text-blue-600">How it works</p>
            <h3 class="mt-3 text-3xl font-black text-[#1A2B5C] md:text-4xl">Safety signals, designed for real life</h3>
          </div>

          <div class="mt-10 grid gap-6 md:grid-cols-3">
            <article class="rounded-2xl border border-slate-200 bg-white p-6 shadow-sm">
              <div class="mb-4 flex h-12 w-12 items-center justify-center rounded-xl bg-blue-100 text-2xl">📍</div>
              <h4 class="text-xl font-bold text-[#1A2B5C]">Map your route</h4>
              <p class="mt-3 text-sm leading-6 text-slate-600">
                Check a neighborhood before walking alone, especially at night or in unfamiliar areas.
              </p>
            </article>

            <article class="rounded-2xl border border-slate-200 bg-white p-6 shadow-sm">
              <div class="mb-4 flex h-12 w-12 items-center justify-center rounded-xl bg-yellow-100 text-2xl">🧠</div>
              <h4 class="text-xl font-bold text-[#1A2B5C]">AI risk scoring</h4>
              <p class="mt-3 text-sm leading-6 text-slate-600">
                We blend lighting, foot traffic, transit patterns, and local reports into a single safety score.
              </p>
            </article>

            <article class="rounded-2xl border border-slate-200 bg-white p-6 shadow-sm">
              <div class="mb-4 flex h-12 w-12 items-center justify-center rounded-xl bg-green-100 text-2xl">🤝</div>
              <h4 class="text-xl font-bold text-[#1A2B5C]">Live community reports</h4>
              <p class="mt-3 text-sm leading-6 text-slate-600">
                Real women share what is happening on the ground, so you can choose a safer route in real time.
              </p>
            </article>
          </div>
        </div>
      </section>

      <section id="safety-map" class="bg-white px-6 py-16 md:px-12">
        <div class="section-shell grid items-center gap-10 lg:grid-cols-[1.2fr_0.8fr]">
          <div>
            <p class="text-sm font-bold uppercase tracking-[0.2em] text-blue-600">Safety map</p>
            <h3 class="mt-3 text-3xl font-black text-[#1A2B5C] md:text-4xl">See the streets women feel safest on</h3>
            <p class="mt-4 max-w-xl text-base leading-7 text-slate-600">
              Compare routes based on visibility, noise, lighting, and verified local reports before you leave home.
            </p>
            <div class="mt-8 rounded-3xl border border-slate-200 bg-slate-50 p-4">
              <div class="grid grid-cols-7 gap-2">
                <div class="h-20 rounded-xl bg-emerald-300"></div>
                <div class="h-20 rounded-xl bg-emerald-200"></div>
                <div class="h-20 rounded-xl bg-yellow-200"></div>
                <div class="h-20 rounded-xl bg-yellow-300"></div>
                <div class="h-20 rounded-xl bg-orange-200"></div>
                <div class="h-20 rounded-xl bg-orange-300"></div>
                <div class="h-20 rounded-xl bg-rose-300"></div>
              </div>
            </div>
          </div>

          <div class="rounded-3xl border border-slate-200 bg-[#1A2B5C] p-6 text-white shadow-xl">
            <p class="text-sm uppercase tracking-[0.2em] text-blue-200">Today</p>
            <div class="mt-4 flex items-baseline gap-2">
              <span class="text-5xl font-black">87</span>
              <span class="text-lg text-blue-200">/100</span>
            </div>
            <p class="mt-3 text-lg font-semibold">Safe route score for central London</p>
            <ul class="mt-6 space-y-3 text-sm text-blue-100">
              <li>• Well-lit streets</li>
              <li>• High foot traffic</li>
              <li>• 3 verified reports this week</li>
              <li>• No recent safety alerts</li>
            </ul>
          </div>
        </div>
      </section>

      <section id="pricing" class="bg-gray-50 px-6 py-16 md:px-12">
        <div class="section-shell">
          <div class="mx-auto max-w-2xl text-center">
            <p class="text-sm font-bold uppercase tracking-[0.2em] text-blue-600">Pricing</p>
            <h3 class="mt-3 text-3xl font-black text-[#1A2B5C] md:text-4xl">Simple, fair pricing</h3>
            <p class="mt-2 text-sm text-slate-500">Pay with your local card, mobile money, or wallet</p>
          </div>

          <div class="mt-10 grid gap-6 md:grid-cols-3">
            <div class="rounded-2xl border border-slate-200 bg-white p-6 shadow-sm">
              <h4 class="text-2xl font-bold text-[#1A2B5C]">Free</h4>
              <p class="mt-3 text-4xl font-black text-[#1A2B5C]">$0</p>
              <p class="mt-2 text-xs text-slate-500">3 safety checks / day</p>
            </div>

            <div class="rounded-2xl border-2 border-[#1A2B5C] bg-[#1A2B5C] p-6 text-white shadow-xl">
              <h4 class="text-2xl font-bold">Pro</h4>
              <p class="mt-3 text-4xl font-black">
                $3.99<span class="text-sm font-normal text-blue-100">/mo</span>
              </p>
              <p class="mt-2 text-xs text-blue-100">Unlimited safety checks and route insights</p>
            </div>

            <div class="rounded-2xl border border-slate-200 bg-white p-6 shadow-sm">
              <h4 class="text-2xl font-bold text-[#1A2B5C]">Guardian</h4>
              <p class="mt-3 text-4xl font-black text-[#1A2B5C]">
                $9.99<span class="text-sm font-normal text-slate-500">/mo</span>
              </p>
              <p class="mt-2 text-xs text-slate-500">Family sharing + live emergency alerts</p>
            </div>
          </div>
        </div>
      </section>
    </main>

    <footer class="bg-[#1A2B5C] px-6 py-8 text-center text-white">
      <p class="text-sm font-bold">
        We never store your exact location. Your data stays encrypted and private.
      </p>
      <p class="mt-2 text-sm text-blue-200">
        © 2026 SheSafe Live • Global safety • Privacy-first • Enterprise security •
        <a href="#" class="underline">Privacy Policy</a>
      </p>
      <div class="mt-4 flex flex-wrap items-center justify-center gap-2 text-sm text-blue-100">
        <span>💳 Visa</span>
        <span>•</span>
        <span>Mastercard</span>
        <span>•</span>
        <span>Local cards</span>
        <span>•</span>
        <span>Mobile money</span>
      </div>
    </footer>

    <script>
      function checkSafety() {
        const box = document.getElementById('resultBox');
        const cityInput = document.getElementById('cityInput');

        if (!box) {
          return;
        }

        const city = cityInput && cityInput.value.trim() ? cityInput.value.trim() : 'Your area';
        const score = 87;
        const locationText = `${city}: ${score}/100 Safe - Well-lit, high foot traffic`;

        const title = document.getElementById('resultTitle');
        const quote = document.getElementById('resultQuote');

        if (title) {
          title.textContent = locationText;
        }

        if (quote) {
          quote.textContent = '"Saved me on my night shift" - Sarah, London';
        }

        box.classList.remove('hidden');
        box.scrollIntoView({ behavior: 'smooth', block: 'start' });
      }

      document.getElementById('checkSafetyBtn')?.addEventListener('click', checkSafety);
    </script>
  </body>
</html>
