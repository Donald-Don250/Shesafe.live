# Shesafe.live
html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SheSafe Live | Safer Streets Before You Walk</title>
  <meta
    name="description"
    content="SheSafe Live combines AI safety analysis, real-time community reports, and privacy-first route protection for women walking alone."
  />
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">
  <style>
    :root {
      --navy: #1A2B5C;
      --navy-2: #132750;
      --ink: #0f172a;
      --muted: #64748b;
      --line: #e2e8f0;
      --bg: #f8fafc;
      --sky: #edf6ff;
      --green: #dcfce7;
      --amber: #fef3c7;
      --rose: #ffe4e6;
      --blue: #2563eb;
    }

    html { scroll-behavior: smooth; }
    body {
      font-family: 'Inter', sans-serif;
      background: var(--bg);
      color: var(--ink);
    }

    .section-shell {
      max-width: 1200px;
      margin: 0 auto;
    }

    .glass {
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
    }

    .shadow-soft {
      box-shadow: 0 28px 65px rgba(15, 23, 42, 0.12);
    }

    .shadow-card {
      box-shadow: 0 16px 32px rgba(15, 23, 42, 0.06);
    }

    .grid-pattern {
      background-image: radial-gradient(rgba(37,99,235,0.08) 1px, transparent 1px);
      background-size: 18px 18px;
    }

    .hero-bg {
      background:
        radial-gradient(circle at top left, rgba(59,130,246,0.16), transparent 24%),
        radial-gradient(circle at bottom right, rgba(251,146,60,0.12), transparent 28%),
        linear-gradient(180deg, #ffffff 0%, #f8fbff 100%);
    }

    .premium-card {
      background: linear-gradient(180deg, #ffffff 0%, #f9fbff 100%);
      border: 1px solid rgba(148,163,184,0.2);
    }

    .app-phone {
      background: linear-gradient(180deg, #f5f9ff 0%, #edf4ff 100%);
      border: 8px solid #0b1120;
      border-radius: 32px;
      overflow: hidden;
    }

    .hud {
      background: linear-gradient(135deg, var(--navy) 0%, #1b366f 100%);
    }

    .input-focus:focus {
      outline: 2px solid rgba(37,99,235,0.2);
      outline-offset: 2px;
    }

    input[type="range"] {
      accent-color: var(--navy);
    }
  </style>
</head>
<body>
  <div class="bg-[#1A2B5C] text-white">
    <div class="section-shell flex items-center justify-center gap-2 px-6 py-2.5 text-center text-[11px] md:text-xs">
      <span class="inline-block h-2.5 w-2.5 rounded-full bg-green-400 animate-pulse"></span>
      <span class="font-bold">LIVE</span>
      <span>Protecting women in 190+ countries • Works offline • Encrypted</span>
    </div>
  </div>

  <header class="sticky top-0 z-50 border-b border-slate-200 bg-white/90 glass">
    <div class="section-shell flex items-center justify-between px-6 py-4 md:px-12">
      <a href="#top" class="flex items-center gap-3">
        <div class="flex h-10 w-10 items-center justify-center rounded-xl bg-blue-100 text-xl">🛡️</div>
        <div class="text-lg font-black tracking-tight text-[#1A2B5C]">SheSafe Live</div>
      </a>

      <nav class="hidden items-center gap-8 text-sm font-medium text-[#1A2B5C] md:flex">
        <a href="#features" class="transition hover:text-blue-600">Features</a>
        <a href="#dashboard" class="transition hover:text-blue-600">Dashboard</a>
        <a href="#stories" class="transition hover:text-blue-600">Stories</a>
        <a href="#pricing" class="transition hover:text-blue-600">Pricing</a>
      </nav>

      <div class="flex items-center gap-3">
        <a href="#pricing" class="hidden rounded-full border border-slate-200 bg-white px-4 py-2 text-sm font-bold text-[#1A2B5C] md:inline-block">Log in</a>
        <a href="#pricing" class="rounded-full bg-[#1A2B5C] px-5 py-2.5 text-sm font-bold text-white">Open App</a>
      </div>
    </div>
  </header>

  <main id="top">
    <section class="hero-bg relative overflow-hidden px-6 py-12 md:px-12 md:py-20">
      <div class="absolute inset-0 grid-pattern opacity-80"></div>
      <div class="section-shell relative grid items-center gap-12 lg:grid-cols-[1.04fr_0.96fr]">
        <div>
          <div class="inline-flex items-center gap-2 rounded-full border border-blue-200 bg-blue-50 px-3 py-1 text-[10px] font-bold uppercase tracking-[0.2em] text-blue-700">
            <span class="inline-block h-2 w-2 rounded-full bg-blue-500"></span>
            Real-time street safety
          </div>

          <h1 class="mt-6 max-w-xl text-5xl font-black leading-[0.92] tracking-[-0.06em] text-[#1A2B5C] md:text-6xl xl:text-7xl">
            Know if a street is safe<br>before you walk it.
          </h1>

          <p class="mt-6 max-w-xl text-lg leading-relaxed text-slate-600">
            AI-powered safety intelligence, trusted local reports, and privacy-first protection for solo walks, night shifts, and unfamiliar places.
          </p>

          <div class="mt-8 flex flex-col gap-3 sm:flex-row">
            <div class="flex flex-1 items-center rounded-full border border-blue-200 bg-white px-4 py-3 shadow-sm">
              <span class="mr-2 text-lg">📍</span>
              <input
                id="cityInput"
                type="text"
                class="input-focus w-full border-none bg-transparent text-sm text-slate-700 outline-none placeholder:text-slate-400"
                placeholder="Your city: London, São Paulo, Tokyo"
              />
            </div>
            <button
              id="checkSafetyBtn"
              class="rounded-full bg-[#1A2B5C] px-6 py-3 text-sm font-bold text-white transition hover:bg-[#20376b]"
            >
              🛡️ Check Safety
            </button>
          </div>

          <div class="mt-4 flex flex-wrap items-center gap-4 text-sm text-slate-500">
            <span>✔ Never sell your exact location</span>
            <span>✔ Works in low-signal areas</span>
            <span>✔ Verified reports</span>
          </div>

          <div id="resultBox" class="mt-6 hidden max-w-lg rounded-3xl border border-green-200 bg-green-50 p-4 shadow-sm">
            <p class="text-[11px] font-bold uppercase tracking-[0.18em] text-green-700">SAFE • LOW RISK • DEMO</p>
            <p id="resultTitle" class="mt-1 text-xl font-black text-slate-900">87/100 Safe — Well-lit, active route</p>
            <p id="resultQuote" class="mt-1 text-xs text-slate-500">“Saved me on my night shift” — Sarah, London</p>
          </div>
        </div>

        <div class="relative">
          <div class="app-phone mx-auto w-[330px] md:w-[360px] shadow-soft">
            <div class="hud px-5 py-4 text-white">
              <div class="flex items-center justify-between text-sm">
                <span class="font-semibold">9:41</span>
                <div class="flex items-center gap-2">
                  <span>📶</span>
                  <span>🔋</span>
                </div>
              </div>

              <div class="mt-5 flex items-center justify-between">
                <div>
                  <p class="text-[10px] uppercase tracking-[0.22em] text-blue-200">Route</p>
                  <p class="mt-1 text-xl font-black">Home → Office</p>
                </div>
                <div class="rounded-full bg-white/10 px-3 py-1 text-[10px] font-bold">LIVE</div>
              </div>

              <div class="mt-5 rounded-2xl bg-white/10 p-3">
                <div class="flex items-center justify-between text-xs text-blue-100">
                  <span>Safety score</span>
                  <span class="font-bold">87/100</span>
                </div>
                <div class="mt-3 h-2.5 w-full rounded-full bg-white/10">
                  <div class="h-2.5 w-[87%] rounded-full bg-gradient-to-r from-emerald-400 via-yellow-300 to-orange-400"></div>
                </div>
              </div>
            </div>

            <div class="bg-white px-4 pb-5 pt-4">
              <div class="rounded-3xl bg-slate-50 p-3">
                <div class="mb-3 flex items-center justify-between">
                  <p class="text-sm font-bold text-slate-700">Map overview</p>
                  <span class="text-[10px] font-bold uppercase tracking-[0.2em] text-emerald-700">safe</span>
                </div>

                <div class="relative h-36 overflow-hidden rounded-2xl bg-[linear-gradient(135deg,#dfeeff,#eff7ff)]">
                  <div class="absolute left-3 top-3 h-16 w-16 rounded-full bg-white/70"></div>
                  <div class="absolute right-4 top-6 h-12 w-16 rounded-full bg-emerald-200/80"></div>
                  <div class="absolute bottom-4 left-4 right-4 flex items-end justify-between gap-2">
                    <div class="w-full rounded-t-xl bg-emerald-300" style="height:40%"></div>
                    <div class="w-full rounded-t-xl bg-yellow-300" style="height:58%"></div>
                    <div class="w-full rounded-t-xl bg-orange-300" style="height:72%"></div>
                    <div class="w-full rounded-t-xl bg-rose-300" style="height:36%"></div>
                  </div>
                </div>
              </div>

              <div class="mt-4 grid grid-cols-3 gap-3">
                <div class="rounded-2xl bg-blue-50 p-3">
                  <div class="text-xl">💡</div>
                  <p class="mt-2 text-[11px] font-bold text-slate-700">Lighting</p>
                  <p class="text-sm font-black text-[#1A2B5C]">92%</p>
                </div>

                <div class="rounded-2xl bg-emerald-50 p-3">
                  <div class="text-xl">👥</div>
                  <p class="mt-2 text-[11px] font-bold text-slate-700">Foot traffic</p>
                  <p class="text-sm font-black text-[#1A2B5C]">78%</p>
                </div>

                <div class="rounded-2xl bg-amber-50 p-3">
                  <div class="text-xl">🚇</div>
                  <p class="mt-2 text-[11px] font-bold text-slate-700">Transit</p>
                  <p class="text-sm font-black text-[#1A2B5C]">81%</p>
                </div>
              </div>

              <div class="mt-4 rounded-2xl border border-slate-200 bg-slate-50 p-3">
                <div class="flex items-center justify-between">
                  <div class="flex items-center gap-2">
                    <div class="flex h-9 w-9 items-center justify-center rounded-full bg-emerald-100 text-lg">🧑‍💼</div>
                    <div>
                      <p class="text-sm font-bold text-slate-700">Trusted contact</p>
                      <p class="text-[11px] text-slate-500">Maya • online</p>
                    </div>
                  </div>
                  <span class="rounded-full bg-emerald-100 px-2 py-1 text-[10px] font-bold uppercase tracking-[0.12em] text-emerald-700">safe</span>
                </div>
              </div>

              <button class="mt-4 w-full rounded-2xl bg-[#1A2B5C] py-3 text-sm font-bold text-white">
                Start Live Share
              </button>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="features" class="bg-slate-50 px-6 py-16 md:px-12">
      <div class="section-shell">
        <div class="mx-auto max-w-3xl text-center">
          <p class="text-sm font-bold uppercase tracking-[0.2em] text-blue-600">Why women trust it</p>
          <h2 class="mt-3 text-3xl font-black text-[#1A2B5C] md:text-4xl">Safety built around real life, not guesswork</h2>
        </div>

        <div class="mt-10 grid gap-6 md:grid-cols-4">
          <div class="premium-card rounded-3xl p-6 shadow-card">
            <div class="mb-4 flex h-12 w-12 items-center justify-center rounded-2xl bg-blue-100 text-2xl">🛡️</div>
            <h3 class="text-lg font-bold text-[#1A2B5C]">Route scoring</h3>
            <p class="mt-2 text-sm leading-6 text-slate-600">Instant insight into lighting, traffic, and how visible a route feels in real time.</p>
          </div>

          <div class="premium-card rounded-3xl p-6 shadow-card">
            <div class="mb-4 flex h-12 w-12 items-center justify-center rounded-2xl bg-violet-100 text-2xl">🔐</div>
            <h3 class="text-lg font-bold text-[#1A2B5C]">Privacy by design</h3>
            <p class="mt-2 text-sm leading-6 text-slate-600">No public exposure, no location resale, and no unnecessary data collection.</p>
          </div>

          <div class="premium-card rounded-3xl p-6 shadow-card">
            <div class="mb-4 flex h-12 w-12 items-center justify-center rounded-2xl bg-emerald-100 text-2xl">📡</div>
            <h3 class="text-lg font-bold text-[#1A2B5C]">Offline-ready</h3>
            <p class="mt-2 text-sm leading-6 text-slate-600">Recent routes and safety notes remain available even when signal drops.</p>
          </div>

          <div class="premium-card rounded-3xl p-6 shadow-card">
            <div class="mb-4 flex h-12 w-12 items-center justify-center rounded-2xl bg-amber-100 text-2xl">🚨</div>
            <h3 class="text-lg font-bold text-[#1A2B5C]">Trusted alerts</h3>
            <p class="mt-2 text-sm leading-6 text-slate-600">A live network of community updates helps identify risky conditions before they escalate.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="dashboard" class="bg-white px-6 py-16 md:px-12">
      <div class="section-shell grid gap-10 lg:grid-cols-[1.15fr_0.85fr]">
        <div class="rounded-[32px] border border-slate-200 bg-slate-50 p-6 shadow-sm md:p-8">
          <div class="mb-6 flex items-center justify-between">
            <div>
              <p class="text-sm font-bold uppercase tracking-[0.2em] text-blue-600">Route risk simulator</p>
              <h2 class="mt-2 text-2xl font-black text-[#1A2B5C]">Check route conditions as you walk</h2>
            </div>
            <div class="rounded-full bg-white px-3 py-1 text-xs font-bold text-slate-700 shadow-sm">Demo</div>
          </div>

          <div class="space-y-5">
            <label class="block">
              <div class="mb-2 flex justify-between text-sm text-slate-600">
                <span>Lighting</span>
                <span id="lightingLabel">80%</span>
              </div>
              <input id="lighting" type="range" min="0" max="100" value="80" class="w-full" />
            </label>

            <label class="block">
              <div class="mb-2 flex justify-between text-sm text-slate-600">
                <span>Foot traffic</span>
                <span id="trafficLabel">70%</span>
              </div>
              <input id="traffic" type="range" min="0" max="100" value="70" class="w-full" />
            </label>

            <label class="block">
              <div class="mb-2 flex justify-between text-sm text-slate-600">
                <span>Transit access</span>
                <span id="transportLabel">65%</span>
              </div>
              <input id="transport" type="range" min="0" max="100" value="65" class="w-full" />
            </label>

            <label class="block">
              <div class="mb-2 flex justify-between text-sm text-slate-600">
                <span>Time of day</span>
                <span id="timeLabel">Night</span>
              </div>
              <select id="timeOfDay" class="w-full rounded-xl border border-slate-200 bg-white px-3 py-2.5 text-sm text-slate-700 outline-none">
                <option value="day">Day</option>
                <option value="evening">Evening</option>
                <option value="night" selected>Night</option>
              </select>
            </label>
          </div>
        </div>

        <div class="rounded-[32px] bg-[#1A2B5C] p-6 text-white shadow-xl md:p-8">
          <p class="text-sm uppercase tracking-[0.2em] text-blue-200">Live result</p>

          <div class="mt-4 flex items-baseline gap-2">
            <span id="scoreValue" class="text-5xl font-black">72</span>
            <span class="text-lg text-blue-200">/100</span>
          </div>

          <div class="mt-4">
            <div class="mb-2 flex items-center justify-between text-sm text-blue-100">
              <span>Risk level</span>
              <span id="riskLevel" class="font-bold">Moderate</span>
            </div>
            <div class="h-2.5 w-full rounded-full bg-white/10">
              <div id="scoreBar" class="h-2.5 rounded-full bg-gradient-to-r from-emerald-400 via-yellow-400 to-orange-500" style="width:72%"></div>
            </div>
          </div>

          <ul class="mt-6 space-y-3 text-sm text-blue-100">
            <li id="routeText">• Route is mostly safe, but visibility drops after dark.</li>
            <li>• Nearby transit access is good.</li>
            <li>• Community reports remain stable.</li>
          </ul>

          <div class="mt-8 rounded-2xl bg-white/5 p-4">
            <p class="text-xs uppercase tracking-[0.2em] text-blue-200">Suggested action</p>
            <p class="mt-2 text-base font-semibold text-white">
              Take the brighter main road and keep a trusted contact updated while walking.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section id="stories" class="bg-[#1A2B5C] px-6 py-16 text-white md:px-12">
      <div class="section-shell">
        <div class="mx-auto max-w-3xl text-center">
          <p class="text-sm font-bold uppercase tracking-[0.2em] text-blue-200">Real experiences</p>
          <h2 class="mt-3 text-3xl font-black md:text-4xl">Safety without sacrificing confidence</h2>
        </div>

        <div class="mt-10 grid gap-6 md:grid-cols-3">
          <div class="rounded-3xl border border-white/10 bg-white/5 p-6">
            <p class="text-lg leading-7 text-blue-50">
              “I used it before my night shift and avoided an isolated stretch. It felt like having a trusted guide in my pocket.”
            </p>
            <div class="mt-5 text-sm text-blue-100">
              <p class="font-bold">Toni S.</p>
              <p>Healthcare worker</p>
            </div>
          </div>

          <div class="rounded-3xl border border-white/10 bg-white/5 p-6">
            <p class="text-lg leading-7 text-blue-50">
              “It helped me choose a brighter route while still feeling confident. I liked that the score was realistic and practical.”
            </p>
            <div class="mt-5 text-sm text-blue-100">
              <p class="font-bold">Aisha M.</p>
              <p>Student commuter</p>
            </div>
          </div>

          <div class="rounded-3xl border border-white/10 bg-white/5 p-6">
            <p class="text-lg leading-7 text-blue-50">
              “The privacy-first design matters. I didn’t feel exposed and I still got meaningful route awareness.”
            </p>
            <div class="mt-5 text-sm text-blue-100">
              <p class="font-bold">Lina R.</p>
              <p>Frequent traveler</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="pricing" class="bg-gray-50 px-6 py-16 md:px-12">
      <div class="section-shell">
        <div class="mx-auto max-w-3xl text-center">
          <p class="text-sm font-bold uppercase tracking-[0.2em] text-blue-600">Simple pricing</p>
          <h2 class="mt-3 text-3xl font-black text-[#1A2B5C] md:text-4xl">Choose the right plan for your routine</h2>
        </div>

        <div class="mt-10 grid gap-6 md:grid-cols-3">
          <div class="rounded-3xl border border-slate-200 bg-white p-6 shadow-card">
            <h3 class="text-2xl font-bold text-[#1A2B5C]">Free</h3>
            <p class="mt-4 text-4xl font-black text-[#1A2B5C]">$0</p>
            <p class="mt-2 text-xs text-slate-500">3 route checks per day</p>
          </div>

          <div class="rounded-3xl border-2 border-[#1A2B5C] bg-[#1A2B5C] p-6 text-white shadow-xl">
            <h3 class="text-2xl font-bold">Pro</h3>
            <p class="mt-4 text-4xl font-black">
              $3.99<span class="text-sm font-normal text-blue-100">/mo</span>
            </p>
            <p class="mt-2 text-xs text-blue-100">Unlimited safety checks + live updates</p>
          </div>

          <div class="rounded-3xl border border-slate-200 bg-white p-6 shadow-card">
            <h3 class="text-2xl font-bold text-[#1A2B5C]">Guardian</h3>
            <p class="mt-4 text-4xl font-black text-[#1A2B5C]">
              $9.99<span class="text-sm font-normal text-slate-500">/mo</span>
            </p>
            <p class="mt-2 text-xs text-slate-500">Trusted contacts + emergency alerts</p>
          </div>
        </div>
      </div>
    </section>

    <section class="bg-white px-6 py-16 md:px-12">
      <div class="section-shell rounded-[32px] border border-slate-200 bg-slate-50 p-8 shadow-sm md:p-10">
        <div class="grid items-center gap-8 md:grid-cols-[1fr_auto]">
          <div>
            <p class="text-sm font-bold uppercase tracking-[0.2em] text-blue-600">Take control</p>
            <h2 class="mt-3 text-3xl font-black text-[#1A2B5C] md:text-4xl">See your route clearly before you step outside.</h2>
          </div>

          <div class="flex flex-col gap-3 sm:flex-row">
            <a href="#pricing" class="rounded-full bg-[#1A2B5C] px-6 py-3 text-sm font-bold text-white">Get started</a>
            <a href="#features" class="rounded-full border border-slate-200 bg-white px-6 py-3 text-sm font-bold text-[#1A2B5C]">Learn more</a>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer class="bg-[#1A2B5C] px-6 py-8 text-center text-white">
    <p class="text-sm font-bold">We never store your exact location. Your data stays encrypted and private.</p>
    <p class="mt-2 text-sm text-blue-200">
      © 2026 SheSafe Live • Global safety • Privacy-first • Enterprise security •
      <a href="#" class="underline">Privacy Policy</a>
    </p>
    <div class="mt-4 flex flex-wrap items-center justify-center gap-3 text-sm text-blue-100">
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
      const title = document.getElementById('resultTitle');
      const quote = document.getElementById('resultQuote');

      if (!box) return;

      const city = cityInput && cityInput.value.trim() ? cityInput.value.trim() : 'Your area';
      const score = 87;

      if (title) title.textContent = `${city}: ${score}/100 Safe — Well-lit, active route`;
      if (quote) quote.textContent = '“Saved me on my night shift” — Sarah, London';

      box.classList.remove('hidden');
      box.scrollIntoView({ behavior: 'smooth', block: 'center' });
    }

    function updateRisk() {
      const lighting = Number(document.getElementById('lighting').value);
      const traffic = Number(document.getElementById('traffic').value);
      const transport = Number(document.getElementById('transport').value);
      const timeOfDay = document.getElementById('timeOfDay').value;

      const timePenalty = timeOfDay === 'night' ? 18 : timeOfDay === 'evening' ? 10 : 0;
      const score = Math.max(0, Math.min(100, Math.round((lighting * 0.35) + (traffic * 0.35) + (transport * 0.2) + (100 - timePenalty) * 0.1)));

      const riskLevel = score >= 80 ? 'Low' : score >= 60 ? 'Moderate' : score >= 40 ? 'Elevated' : 'High';

      document.getElementById('lightingLabel').textContent = `${lighting}%`;
      document.getElementById('trafficLabel').textContent = `${traffic}%`;
      document.getElementById('transportLabel').textContent = `${transport}%`;
      document.getElementById('timeLabel').textContent = timeOfDay.charAt(0).toUpperCase() + timeOfDay.slice(1);

      document.getElementById('scoreValue').textContent = score;
      document.getElementById('riskLevel').textContent = riskLevel;
      document.getElementById('scoreBar').style.width = `${score}%`;

      const routeText = document.getElementById('routeText');
      if (routeText) {
        if (riskLevel === 'Low') {
          routeText.textContent = '• Route is well-lit and active, making it ideal for walking after dark.';
        } else if (riskLevel === 'Moderate') {
          routeText.textContent = '• Route is mostly safe, but visibility drops after dark.';
        } else if (riskLevel === 'Elevated') {
          routeText.textContent = '• Route has limited visibility and fewer people around after dark.';
        } else {
          routeText.textContent = '• Route may be unsafe. Consider another path or share your location with a trusted contact.';
        }
      }
    }

    const checkBtn = document.getElementById('checkSafetyBtn');
    if (checkBtn) checkBtn.addEventListener('click', checkSafety);

    ['lighting', 'traffic', 'transport', 'timeOfDay'].forEach((id) => {
      const el = document.getElementById(id);
      if (el) {
        el.addEventListener('input', updateRisk);
        el.addEventListener('change', updateRisk);
      }
    });

    updateRisk();
  </script>
</body>
</html>