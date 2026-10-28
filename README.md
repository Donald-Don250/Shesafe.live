# Shesafe.live
html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SheSafe Live - Know if a street is safe BEFORE you walk it</title>
<script src="https://cdn.tailwindcss.com"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700;800;900&display=swap" rel="stylesheet">
<style>body{font-family:'Inter',sans-serif}</style>
</head>
<body class="bg-white">

<!-- LIVE BAR -->
<div class="bg-[#1A2B5C] text-white text- md:text-xs px-6 py-2.5 flex items-center gap-2">
<span class="text-green-400">●</span><span class="font-bold">LIVE:</span><span>Protecting women in 190+ countries • Works offline • Encrypted</span>
</div>

<!-- HEADER -->
<header class="flex justify-between items-center px-6 md:px-12 py-4 bg-white sticky top-0 z-50 border-b border-gray-100">
<div class="flex items-center gap-2">
<div class="w-8 h-8 bg-blue-100 rounded-lg flex items-center justify-center">🛡️</div>
<h1 class="font-black text-xl md:text-2xl text-[#1A2B5C]">SheSafe Live</h1>
</div>
<div class="hidden md:flex gap-8 text-sm font-medium text-[#1A2B5C]"><a href="#">How it works</a><a href="#">Safety Map</a><a href="#pricing">Pricing</a></div>
<a href="#pricing" class="bg-[#1A2B5C] text-white px-5 py-2.5 rounded-lg font-bold text-sm">Open App</a>
</header>

<!-- HERO -->
<section class="px-6 md:px-12 py-12 md:py-20 bg-white">
<div class="max-w-7xl mx-auto grid md:grid-cols-2 gap-12 items-center">
<div>
<h1 class="text-5xl md:text-6xl font-black leading-[0.95] tracking-tight text-[#1A2B5C]">Know if a street is safe<br>BEFORE you walk it</h1>
<p class="mt-6 text-gray-600 text-lg leading-relaxed max-w-xl">AI-powered safety insights + real women reporting live. For solo walks, night shifts, new cities.</p>

<div class="mt-8 flex gap-3 max-w-lg">
<div class="flex-1 flex items-center border border-blue-200 rounded-full px-4 py-3 bg-blue-50/50"><span class="mr-2">📍</span><input id="cityInput" placeholder="Your city: London, São Paulo, Tokyo..." class="bg-transparent outline-none w-full text-sm"></div>
<button onclick="checkSafety()" class="bg-[#1A2B5C] text-white px-6 py-3 rounded-full font-bold text-sm">🛡️ Check Safety</button>
</div>
<p class="mt-3 text- text-gray-500">Enterprise-grade security • We never sell your location</p>

<!-- FIXED DEMO RESULT - NO RANDOM -->
<div id="resultBox" class="hidden mt-6 bg-green-50 border border-green-200 p-4 rounded-2xl max-w-lg">
<p class="text-xs font-bold text-green-700">SAFE • Low risk • Demo</p>
<p class="text-xl font-black mt-1">87/100 Safe - Well-lit, high foot traffic</p>
<p class="text-xs text-gray-500 mt-1">"Saved me on my night shift" - Sarah, London</p>
</div>
</div>

<div class="flex justify-center">
<div class="w-[300px] h-[550px] bg-[#1A2B5C] rounded- p-3 shadow-2xl border-[8px] border-black">
<div class="bg-[#E0E6F0] h-full rounded- overflow-hidden relative">
<div class="bg-white m-3 p-3 rounded-xl shadow"><p class="text- font-bold bg-[#1A2B5C] text-white px-2 py-1 rounded inline-block">Live Map • 190+ countries</p></div>
<div class="absolute bottom-4 left-4 right-4"><button class="w-full bg-[#1A2B5C] text-white py-3 rounded-xl font-bold text-sm">Start Live Share</button></div>
</div>
</div>
</div>
</div>
</section>

<!-- PRICING BACK - GLOBAL -->
<section id="pricing" class="px-6 md:px-12 py-16 bg-gray-50">
<div class="max-w-5xl mx-auto">
<h2 class="text-3xl font-black text-center text-[#1A2B5C]">Simple, fair pricing</h2>
<p class="text-center text-gray-500 text-sm mt-2">Pay with your local card, mobile money, or wallet</p>
<div class="grid md:grid-cols-3 gap-6 mt-10">
<div class="bg-white p-6 rounded-2xl border"><h3 class="font-bold">Free</h3><p class="text-3xl font-black mt-2">$0</p><p class="text-xs text-gray-500 mt-2">3 safety checks / day</p></div>
<div class="bg-[#1A2B5C] text-white p-6 rounded-2xl border-2 border-[#1A2B5C]"><h3 class="font-bold">Pro</h3><p class="text-3xl font-black mt-2">$3.99<span class="text-sm font-normal">/mo</span></p><p class="text-xs text-blue-200 mt-2">Unlimited checks + Live share + Offline mode</p><button class="mt-4 w-full bg-white text-[#1A2B5C] py-2 rounded-lg font-bold text-sm">Get Pro - Local payment</button></div>
<div class="bg-white p-6 rounded-2xl border"><h3 class="font-bold">Guardian</h3><p class="text-3xl font-black mt-2">$9.99<span class="text-sm font-normal">/mo</span></p><p class="text-xs text-gray-500 mt-2">Family plan + 24/7 alerts</p></div>
</div>
</div>
</section>

<!-- TRUST FOOTER -->
<footer class="bg-[#1A2B5C] text-white px-6 py-8 text-center">
<p class="text-sm font-bold">We never store your exact location. Your data stays encrypted and private.</p>
<p class="text- text-blue-200 mt-2">© 2026 SheSafe Live • Global safety • Privacy-first • Enterprise security • <a href="#" class="underline">Privacy Policy</a></p>
<div class="flex justify-center gap-2 mt-3 text-"><span>💳 Visa</span><span>•</span><span>Mastercard</span><span>•</span><span>Local cards</span><span>•</span><span>Mobile money</span></div>
</footer>

<script>
function checkSafety(){
  const box = document.getElementById('resultBox');
  box.classList.remove('hidden');
  box.scrollIntoView({behavior:'smooth'});
}
</script>
</body>
</html>

