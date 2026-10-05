<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Samy Imanes | Fotos Imantadas 5x5 cm en Puerto Montt</title>
<!-- Tailwind CSS -->
<script src="https://cdn.tailwindcss.com"></script>
<!-- Google Fonts: Poppins & Bubblegum Sans -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bubblegum+Sans&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<!-- Lucide Icons -->
<script src="https://unpkg.com/lucide@latest"></script>
<script>
tailwind.config = {
theme: {
extend: {
colors: {
samy: {
pink: '#FFB6C1',
lightpink: '#FFF0F5',
darkpink: '#FF69B4',
purple: '#E6E6FA',
deepPurple: '#9370DB',
yellow: '#FFFACD',
warmYellow: '#FFE4B5',
mint: '#E0F8E7',
text: '#4A4A4A'
}
},
fontFamily: {
sans: ['Poppins', 'sans-serif'],
fun: ['Bubblegum Sans', 'cursive']
}
}
}
}
</script>
<style>
.custom-scrollbar::-webkit-scrollbar {
width: 6px;
}
.custom-scrollbar::-webkit-scrollbar-track {
background: #FFF0F5;
}
.custom-scrollbar::-webkit-scrollbar-thumb {
background: #FFB6C1;
border-radius: 10px;
}
.magnet-shadow {
box-shadow: 0 10px 25px -5px rgba(255, 105, 180, 0.25), 0 8px 10px -6px rgba(147, 112, 219, 0.15);
}
.magnet-frame {
box-shadow: 0 6px 18px rgba(0,0,0,0.08);
transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}
.magnet-frame:hover {
transform: translateY(-4px) scale(1.02);
}
@keyframes float {
0%, 100% { transform: translateY(0px) rotate(0deg); }
50% { transform: translateY(-8px) rotate(1.5deg); }
}
.floating {
animation: float 4s ease-in-out infinite;
}
</style>
</head>
<body class="bg-samy-lightpink text-samy-text font-sans selection:bg-samy-pink selection:text-white flex flex-col min-h-screen">
<!-- Top Announcement Bar -->
<div class="bg-gradient-to-r from-samy-darkpink via-samy-deepPurple to-samy-darkpink text-white text-xs md:text-sm py-2 px-4 text-center font-medium shadow-sm flex items-center justify-center gap-2">
<i data-lucide="map-pin" class="w-4 h-4"></i>
<span>📍 Desde <strong>Puerto Montt, Región de Los Lagos</strong> para todo Chile 🇨🇱 | Imanes 5x5 cm de Alta Calidad</span>
</div>
<!-- Navigation Bar -->
<header class="sticky top-0 z-40 bg-white/95 backdrop-blur-md shadow-sm border-b border-samy-pink/30">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="flex items-center justify-between h-20">

<!-- Logo -->
<a href="#" class="flex items-center gap-3 group">
<div class="w-12 h-12 rounded-2xl bg-gradient-to-tr from-samy-darkpink to-samy-deepPurple flex items-center justify-center text-white text-2xl font-fun font-bold shadow-md transform group-hover:rotate-6 transition">
🧲
</div>
<div>
<span class="font-fun text-3xl tracking-wide bg-gradient-to-r from-samy-darkpink to-samy-deepPurple bg-clip-text text-transparent block leading-none">Samy Imanes</span>
<span class="text-[10px] uppercase tracking-widest text-gray-500 font-bold block mt-0.5">Puerto Montt • Todos 5x5 cm</span>
</div>
</a>
<!-- Desktop Navigation Menu -->
<nav class="hidden md:flex items-center space-x-8 font-medium text-sm">
<a href="#packs" class="hover:text-samy-darkpink transition flex items-center gap-1.5"><i data-lucide="grid" class="w-4 h-4"></i> Packs de Imanes</a>
<a href="#personalizador" class="hover:text-samy-darkpink transition flex items-center gap-1.5 text-samy-darkpink font-bold"><i data-lucide="wand-2" class="w-4 h-4"></i> Personalizador 5x5</a>
<a href="#nosotras" class="hover:text-samy-darkpink transition flex items-center gap-1.5"><i data-lucide="heart" class="w-4 h-4"></i> Sobre Nosotras</a>
<a href="#faq" class="hover:text-samy-darkpink transition flex items-center gap-1.5"><i data-lucide="help-circle" class="w-4 h-4"></i> Preguntas</a>
</nav>
<!-- Actions / Cart Button -->
<div class="flex items-center space-x-3">
<a href="https://www.instagram.com/samy_imanes/" target="_blank" class="hidden sm:flex items-center gap-1.5 bg-samy-purple/40 hover:bg-samy-purple text-samy-deepPurple px-3 py-2 rounded-xl text-xs font-semibold transition">
<i data-lucide="instagram" class="w-4 h-4"></i>
<span>@samy_imanes</span>
</a>

<button onclick="toggleCart()" class="relative bg-samy-pink/25 hover:bg-samy-pink/40 text-samy-darkpink p-3 rounded-2xl transition shadow-sm flex items-center justify-center group">
<i data-lucide="shopping-bag" class="w-5 h-5 transform group-hover:scale-110 transition"></i>
<span id="cart-badge" class="absolute -top-1.5 -right-1.5 bg-samy-darkpink text-white text-xs font-bold w-5 h-5 rounded-full flex items-center justify-center border-2 border-white shadow-sm">0</span>
</button>
<button onclick="toggleMobileMenu()" class="md:hidden p-2 rounded-xl text-gray-600 hover:text-samy-darkpink hover:bg-samy-lightpink">
<i data-lucide="menu" class="w-6 h-6"></i>
</button>
</div>
</div>
</div>
<!-- Mobile Dropdown Menu -->
<div id="mobile-menu" class="hidden md:hidden bg-white border-b border-samy-pink/20 px-4 pt-2 pb-4 space-y-2">
<a href="#packs" onclick="toggleMobileMenu()" class="block px-3 py-2 rounded-xl hover:bg-samy-lightpink font-medium text-sm">Packs Oficiales 5x5 cm</a>
<a href="#personalizador" onclick="toggleMobileMenu()" class="block px-3 py-2 rounded-xl hover:bg-samy-lightpink text-samy-darkpink font-bold text-sm">Diseñador Interactivo</a>
<a href="#nosotras" onclick="toggleMobileMenu()" class="block px-3 py-2 rounded-xl hover:bg-samy-lightpink text-sm">Sobre Samy Imanes (Puerto Montt)</a>
<a href="#faq" onclick="toggleMobileMenu()" class="block px-3 py-2 rounded-xl hover:bg-samy-lightpink text-sm">Preguntas Frecuentes</a>
<a href="https://www.instagram.com/samy_imanes/" target="_blank" class="flex items-center gap-2 px-3 py-2 rounded-xl bg-samy-purple/30 text-samy-deepPurple text-xs font-bold">
<i data-lucide="instagram" class="w-4 h-4"></i>
Visitar @samy_imanes en Instagram
</a>
</div>
</header>
<!-- Hero Section -->
<section class="relative overflow-hidden bg-gradient-to-b from-white via-samy-lightpink/60 to-samy-purple/20 py-12 lg:py-20">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">

<!-- Left Hero Column -->
<div class="space-y-6 text-center lg:text-left">
<div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-samy-pink/30 text-samy-darkpink text-xs sm:text-sm font-bold shadow-sm">
<i data-lucide="sparkles" class="w-4 h-4"></i>
<span>Medida Única Estándar: 5 cm x 5 cm</span>
</div>
<h1 class="text-4xl sm:text-5xl lg:text-6xl font-fun text-gray-800 leading-tight">
Tus mejores fotos convertidas en <span class="bg-gradient-to-r from-samy-darkpink to-samy-deepPurple bg-clip-text text-transparent">Imanes Cuadrados 5x5 cm</span>
</h1>
<p class="text-gray-600 text-base sm:text-lg max-w-xl mx-auto lg:mx-0">
Impresión fotográfica de alta nitidez con lámina de imán completa en la parte trasera. Elaborados con amor en <strong>Puerto Montt</strong> para rellenar tu refrigerador de recuerdos mágicos.
</p>
<div class="flex flex-col sm:flex-row gap-4 justify-center lg:justify-start pt-2">
<a href="#personalizador" class="bg-samy-darkpink hover:bg-pink-600 text-white font-bold px-8 py-4 rounded-2xl shadow-lg hover:shadow-xl transition-all transform hover:-translate-y-0.5 flex items-center justify-center gap-2">
<i data-lucide="wand-2" class="w-5 h-5"></i>
Diseñar mi Pack 5x5
</a>
<a href="#packs" class="bg-white hover:bg-samy-purple/30 text-samy-deepPurple border-2 border-samy-purple font-bold px-8 py-4 rounded-2xl transition-all flex items-center justify-center gap-2 shadow-sm">
<i data-lucide="grid" class="w-5 h-5"></i>
Ver Precios y Packs
</a>
</div>
<!-- Location Badge & Guarantee -->
<div class="pt-6 border-t border-samy-pink/30 flex flex-wrap justify-center lg:justify-start gap-6 text-xs text-gray-600">
<div class="flex items-center gap-2">
<div class="w-8 h-8 rounded-full bg-samy-mint flex items-center justify-center text-emerald-600">
<i data-lucide="check-circle-2" class="w-4 h-4"></i>
</div>
<div class="text-left">
<p class="font-bold text-gray-800">100% Imantados</p>
<p class="text-[11px]">Reverso completo</p>
</div>
</div>
<div class="flex items-center gap-2">
<div class="w-8 h-8 rounded-full bg-samy-warmYellow flex items-center justify-center text-amber-700">
<i data-lucide="map-pin" class="w-4 h-4"></i>
</div>
<div class="text-left">
<p class="font-bold text-gray-800">Puerto Montt</p>
<p class="text-[11px]">Envíos a todo Chile</p>
</div>
</div>
</div>
</div>
<!-- Right Visual Floating Magnets Preview -->
<div class="relative flex justify-center items-center">
<div class="absolute w-72 h-72 bg-samy-pink/30 rounded-full blur-3xl -top-6 -left-6"></div>
<div class="absolute w-72 h-72 bg-samy-purple/40 rounded-full blur-3xl -bottom-6 -right-6"></div>
<!-- 5x5 cm Magnets Grid Mockup -->
<div class="relative grid grid-cols-2 sm:grid-cols-3 gap-3 p-4 bg-white/70 backdrop-blur-md rounded-3xl border border-samy-pink/30 magnet-shadow max-w-md w-full">

<div class="magnet-frame bg-white p-2 rounded-2xl border border-gray-100 flex flex-col items-center">
<img src="https://images.unsplash.com/photo-1511895426328-dc8714191300?auto=format&fit=crop&w=300&q=80" alt="Foto 1" class="w-full aspect-square object-cover rounded-xl">
<span class="text-[10px] font-bold text-gray-500 mt-1.5">5 x 5 cm</span>
</div>
<div class="magnet-frame bg-white p-2 rounded-2xl border border-gray-100 flex flex-col items-center">
<img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=300&q=80" alt="Foto 2" class="w-full aspect-square object-cover rounded-xl">
<span class="text-[10px] font-bold text-gray-500 mt-1.5">5 x 5 cm</span>
</div>
<div class="magnet-frame bg-white p-2 rounded-2xl border border-gray-100 flex flex-col items-center">
<img src="https://images.unsplash.com/photo-1517841905240-472988babdf9?auto=format&fit=crop&w=300&q=80" alt="Foto 3" class="w-full aspect-square object-cover rounded-xl">
<span class="text-[10px] font-bold text-gray-500 mt-1.5">5 x 5 cm</span>
</div>
<div class="magnet-frame bg-white p-2 rounded-2xl border border-gray-100 flex flex-col items-center">
<img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?auto=format&fit=crop&w=300&q=80" alt="Foto 4" class="w-full aspect-square object-cover rounded-xl">
<span class="text-[10px] font-bold text-gray-500 mt-1.5">5 x 5 cm</span>
</div>
<div class="magnet-frame bg-white p-2 rounded-2xl border border-gray-100 flex flex-col items-center">
<img src="https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=300&q=80" alt="Foto 5" class="w-full aspect-square object-cover rounded-xl">
<span class="text-[10px] font-bold text-gray-500 mt-1.5">5 x 5 cm</span>
</div>
<div class="magnet-frame bg-samy-pink/20 p-2 rounded-2xl border border-samy-pink flex flex-col items-center justify-center text-center p-2">
<span class="text-2xl">✨</span>
<span class="font-fun text-sm text-samy-darkpink font-bold">Pack x12</span>
<span class="text-[9px] text-gray-600">$16.990</span>
</div>
</div>
</div>
</div>
</div>
</section>
<!-- Interactive Personalizer (Simulador 5x5 cm) -->
<section id="personalizador" class="py-16 bg-white relative">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="text-center max-w-3xl mx-auto mb-10">
<span class="bg-samy-purple text-samy-deepPurple px-4 py-1.5 rounded-full text-xs font-bold uppercase tracking-wider">Simulador 5cm x 5cm</span>
<h2 class="text-3xl sm:text-4xl font-fun text-gray-800 mt-2">Diseña y Previsualiza tu Imán</h2>
<p class="text-gray-600 mt-2">Prueba cómo quedará el formato cuadrado perfecto de 5x5 cm antes de coordinar tus fotos.</p>
</div>
<div class="bg-samy-lightpink/70 rounded-3xl p-6 lg:p-10 border border-samy-pink/30 shadow-xl grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">

<!-- Left Controls -->
<div class="lg:col-span-6 space-y-6">

<!-- Step 1: Choose Pack -->
<div>
<label class="block font-bold text-gray-800 mb-2 flex items-center gap-2 text-sm">
<span class="w-6 h-6 rounded-full bg-samy-darkpink text-white text-xs flex items-center justify-center font-bold">1</span>
Elige el Pack Deseado
</label>
<select id="sim-pack-select" onchange="updateSimPack()" class="w-full px-4 py-3 rounded-2xl border border-samy-pink focus:ring-2 focus:ring-samy-darkpink focus:outline-none text-sm font-semibold bg-white text-gray-800 shadow-sm">
<option value="6">Pack 6 imanes 5x5 cm — $9.990</option>
<option value="9">Pack 9 imanes 5x5 cm — $13.990</option>
<option value="12" selected>Pack 12 imanes 5x5 cm — $16.990 ⭐ Mas vendido</option>
<option value="18">Pack 18 imanes 5x5 cm — $24.990</option>
<option value="24">Pack 24 imanes 5x5 cm — $32.990 🔥 Mejor valor</option>
</select>
</div>
<!-- Step 2: Image Selection -->
<div>
<label class="block font-bold text-gray-800 mb-2 flex items-center gap-2 text-sm">
<span class="w-6 h-6 rounded-full bg-samy-darkpink text-white text-xs flex items-center justify-center font-bold">2</span>
Prueba con tu Foto
</label>
<div class="flex flex-col sm:flex-row gap-3">
<label class="cursor-pointer flex-1 bg-white border-2 border-dashed border-samy-pink hover:border-samy-darkpink rounded-2xl p-3 text-center transition flex items-center justify-center gap-2 text-samy-darkpink font-bold text-sm shadow-sm">
<i data-lucide="upload-cloud" class="w-5 h-5"></i>
<span>Subir Imagen</span>
<input type="file" id="user-photo-input" accept="image/*" class="hidden" onchange="handleImageUpload(event)">
</label>
<button onclick="setSamplePhoto('https://images.unsplash.com/photo-1511895426328-dc8714191300?auto=format&fit=crop&w=400&q=80')" class="bg-white border border-gray-200 px-3 py-2 rounded-2xl text-xs hover:bg-samy-purple/30 font-semibold text-gray-600 transition shadow-sm">Muestra 1</button>
<button onclick="setSamplePhoto('https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=400&q=80')" class="bg-white border border-gray-200 px-3 py-2 rounded-2xl text-xs hover:bg-samy-purple/30 font-semibold text-gray-600 transition shadow-sm">Muestra 2</button>
</div>
</div>
<!-- Step 3: Optional Text / Date -->
<div>
<label class="block font-bold text-gray-800 mb-2 flex items-center gap-2 text-sm">
<span class="w-6 h-6 rounded-full bg-samy-darkpink text-white text-xs flex items-center justify-center font-bold">3</span>
Texto o Fecha (Opcional en la foto)
</label>
<input type="text" id="sim-text-input" oninput="updateSimText()" placeholder="Ej: Cancún 2024 ❤️ o Bautizo Sofía" class="w-full px-4 py-3 rounded-2xl border border-gray-200 focus:ring-2 focus:ring-samy-darkpink focus:outline-none text-sm bg-white shadow-sm">
</div>
<!-- Summary & Add Button -->
<div class="pt-2 border-t border-samy-pink/30 flex items-center justify-between">
<div>
<span class="text-xs text-gray-500 block">Precio del Pack Seleccionado:</span>
<span id="sim-price-tag" class="text-2xl font-fun text-samy-darkpink font-bold">$16.990</span>
</div>
<button onclick="addSimulatedPackToCart()" class="bg-gradient-to-r from-samy-darkpink to-samy-deepPurple hover:from-pink-600 hover:to-purple-700 text-white font-bold px-6 py-3.5 rounded-2xl shadow-lg transition flex items-center gap-2 text-sm">
<i data-lucide="shopping-cart" class="w-5 h-5"></i>
Agregar Pack al Carrito
</button>
</div>
</div>
<!-- Right Live Preview -->
<div class="lg:col-span-6 flex flex-col items-center justify-center bg-gradient-to-tr from-samy-purple/40 to-samy-pink/30 rounded-3xl p-6 min-h-[380px] border border-white">
<div class="flex items-center gap-2 bg-white/80 px-3 py-1 rounded-full text-xs font-bold text-samy-deepPurple mb-4 shadow-sm">
<i data-lucide="ruler" class="w-4 h-4"></i>
<span>Proporción Exacta Cuadrada (5 cm x 5 cm)</span>
</div>
<!-- 5x5 Frame Container -->
<div class="relative bg-white p-3 rounded-2xl shadow-2xl magnet-shadow border border-gray-100 w-60 h-60 flex flex-col items-center justify-center group">
<div class="w-full h-full relative overflow-hidden rounded-xl bg-gray-100 flex items-center justify-center">
<img id="sim-preview-img" src="https://images.unsplash.com/photo-1511895426328-dc8714191300?auto=format&fit=crop&w=500&q=80" alt="Previsualización Imán 5x5" class="w-full h-full object-cover">

<!-- Overlay Text -->
<div id="sim-text-overlay" class="absolute bottom-2 left-2 right-2 bg-black/50 backdrop-blur-xs text-white text-[11px] font-semibold text-center py-1 px-2 rounded-lg truncate hidden">
Cancún 2024 ❤️
</div>
</div>
<!-- Size Badge Overlay -->
<span class="absolute -top-3 -right-3 bg-samy-darkpink text-white text-[10px] font-bold px-2.5 py-1 rounded-full shadow-md">
5 x 5 cm
</span>
</div>
<p class="text-xs text-gray-600 mt-5 text-center font-medium max-w-xs">
📸 <em>Tus fotos impresas tendrán esta misma nitidez y bordes ajustados a 5x5 cm.</em>
</p>
</div>
</div>
</div>
</section>
<!-- Official Packs Grid Catalog -->
<section id="packs" class="py-16 bg-samy-lightpink/40">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="text-center max-w-3xl mx-auto mb-12">
<span class="bg-samy-pink/30 text-samy-darkpink px-4 py-1.5 rounded-full text-xs font-bold uppercase tracking-wider">Opciones Únicas Disponibles</span>
<h2 class="text-3xl sm:text-4xl font-fun text-gray-800 mt-2">Nuestros Packs Oficiales de Imanes 5x5 cm</h2>
<p class="text-gray-600 mt-1 text-sm sm:text-base">Elige la cantidad de fotos que deseas imantar. Todos incluyen impresión fotográfica brillante de 5x5 cm con reverso imantado total.</p>
</div>
<!-- Packs Grid -->
<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">

<!-- Pack 6 -->
<div class="bg-white rounded-3xl p-6 border border-samy-pink/30 shadow-sm hover:shadow-md transition flex flex-col justify-between relative">
<div>
<div class="w-12 h-12 rounded-2xl bg-samy-purple/40 text-samy-deepPurple flex items-center justify-center font-fun text-2xl font-bold mb-4">
6
</div>
<h3 class="font-fun text-2xl text-gray-800">Pack 6 Imanes 5x5 cm</h3>
<p class="text-xs text-gray-500 mt-1">Ideal para un detalle rápido o regalo tierno con fotos de tu galería.</p>
<ul class="mt-4 space-y-2 text-xs text-gray-600">
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-emerald-500"></i> 6 Fotografías de 5 cm x 5 cm</li>
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-emerald-500"></i> Imán completo en la espalda</li>
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-emerald-500"></i> Presentación lista para regalar</li>
</ul>
</div>
<div class="pt-6 mt-6 border-t border-gray-100 flex items-center justify-between">
<span class="text-2xl font-fun text-samy-darkpink font-bold">$9.990</span>
<button onclick="addPackToCart(6, 6990)" class="bg-samy-pink/20 hover:bg-samy-darkpink text-samy-darkpink hover:text-white px-4 py-2.5 rounded-xl font-bold text-xs transition flex items-center gap-1.5">
<i data-lucide="plus" class="w-4 h-4"></i> Elegir Pack
</button>
</div>
</div>
<!-- Pack 9 -->
<div class="bg-white rounded-3xl p-6 border border-samy-pink/30 shadow-sm hover:shadow-md transition flex flex-col justify-between relative">
<div>
<div class="w-12 h-12 rounded-2xl bg-samy-purple/40 text-samy-deepPurple flex items-center justify-center font-fun text-2xl font-bold mb-4">
9
</div>
<h3 class="font-fun text-2xl text-gray-800">Pack 9 Imanes 5x5 cm</h3>
<p class="text-xs text-gray-500 mt-1">Perfecto para formar una cuadrícula perfecta de 3x3 en tu refrigerador.</p>
<ul class="mt-4 space-y-2 text-xs text-gray-600">
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-emerald-500"></i> 9 Fotografías de 5 cm x 5 cm</li>
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-emerald-500"></i> Excelente para collage estilo Instagram</li>
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-emerald-500"></i> Colores vivos y duraderos</li>
</ul>
</div>
<div class="pt-6 mt-6 border-t border-gray-100 flex items-center justify-between">
<span class="text-2xl font-fun text-samy-darkpink font-bold">$13.990</span>
<button onclick="addPackToCart(9, 12990)" class="bg-samy-pink/20 hover:bg-samy-darkpink text-samy-darkpink hover:text-white px-4 py-2.5 rounded-xl font-bold text-xs transition flex items-center gap-1.5">
<i data-lucide="plus" class="w-4 h-4"></i> Elegir Pack
</button>
</div>
</div>
<!-- Pack 12 (Destacado - Más vendido) -->
<div class="bg-gradient-to-b from-white to-samy-lightpink rounded-3xl p-6 border-2 border-samy-darkpink shadow-lg hover:shadow-xl transition flex flex-col justify-between relative transform lg:-translate-y-2">
<span class="absolute -top-3 right-6 bg-samy-darkpink text-white text-[10px] font-bold uppercase tracking-widest px-3 py-1 rounded-full shadow-sm">
⭐ El más vendido
</span>
<div>
<div class="w-12 h-12 rounded-2xl bg-samy-darkpink text-white flex items-center justify-center font-fun text-2xl font-bold mb-4 shadow-md">
12
</div>
<h3 class="font-fun text-2xl text-gray-800">Pack 12 Imanes 5x5 cm</h3>
<p class="text-xs text-gray-500 mt-1">El equilibrio perfecto para resumir un año completo de recuerdos o vacaciones.</p>
<ul class="mt-4 space-y-2 text-xs text-gray-700 font-medium">
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-samy-darkpink"></i> 12 Fotografías de 5 cm x 5 cm</li>
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-samy-darkpink"></i> El favorito de nuestras clientas</li>
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-samy-darkpink"></i> Empaque decorativo especial</li>
</ul>
</div>
<div class="pt-6 mt-6 border-t border-samy-pink/30 flex items-center justify-between">
<span class="text-2xl font-fun text-samy-darkpink font-bold">$16.990</span>
<button onclick="addPackToCart(12, 16990)" class="bg-samy-darkpink hover:bg-pink-600 text-white px-5 py-2.5 rounded-xl font-bold text-xs transition flex items-center gap-1.5 shadow-md">
<i data-lucide="plus" class="w-4 h-4"></i> Elegir Pack
</button>
</div>
</div>
<!-- Pack 18 -->
<div class="bg-white rounded-3xl p-6 border border-samy-pink/30 shadow-sm hover:shadow-md transition flex flex-col justify-between relative">
<div>
<div class="w-12 h-12 rounded-2xl bg-samy-purple/40 text-samy-deepPurple flex items-center justify-center font-fun text-2xl font-bold mb-4">
18
</div>
<h3 class="font-fun text-2xl text-gray-800">Pack 18 Imanes 5x5 cm</h3>
<p class="text-xs text-gray-500 mt-1">Ideal para regalar a abuelos o llenar espacios grandes con recuerdos de la familia.</p>
<ul class="mt-4 space-y-2 text-xs text-gray-600">
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-emerald-500"></i> 18 Fotografías de 5 cm x 5 cm</li>
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-emerald-500"></i> Excelente precio por unidad</li>
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-emerald-500"></i> Alta resolución garantizada</li>
</ul>
</div>
<div class="pt-6 mt-6 border-t border-gray-100 flex items-center justify-between">
<span class="text-2xl font-fun text-samy-darkpink font-bold">$24.990</span>
<button onclick="addPackToCart(18, 24990)" class="bg-samy-pink/20 hover:bg-samy-darkpink text-samy-darkpink hover:text-white px-4 py-2.5 rounded-xl font-bold text-xs transition flex items-center gap-1.5">
<i data-lucide="plus" class="w-4 h-4"></i> Elegir Pack
</button>
</div>
</div>
<!-- Pack 24 (Mejor Valor) -->
<div class="bg-white rounded-3xl p-6 border-2 border-samy-purple shadow-sm hover:shadow-md transition flex flex-col justify-between relative sm:col-span-2 lg:col-span-1">
<span class="absolute -top-3 right-6 bg-samy-deepPurple text-white text-[10px] font-bold uppercase tracking-widest px-3 py-1 rounded-full shadow-sm">
🔥 Mejor Valor
</span>
<div>
<div class="w-12 h-12 rounded-2xl bg-samy-purple text-samy-deepPurple flex items-center justify-center font-fun text-2xl font-bold mb-4">
24
</div>
<h3 class="font-fun text-2xl text-gray-800">Pack 24 Imanes 5x5 cm</h3>
<p class="text-xs text-gray-500 mt-1">La colección definitiva para los amantes de las fotos o souvenirs de eventos.</p>
<ul class="mt-4 space-y-2 text-xs text-gray-600">
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-samy-deepPurple"></i> 24 Fotografías de 5 cm x 5 cm</li>
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-samy-deepPurple"></i> Mayor ahorro por imán</li>
<li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-samy-deepPurple"></i> Envío prioritario</li>
</ul>
</div>
<div class="pt-6 mt-6 border-t border-gray-100 flex items-center justify-between">
<span class="text-2xl font-fun text-samy-darkpink font-bold">$32.990</span>
<button onclick="addPackToCart(24, 32990)" class="bg-samy-purple/40 hover:bg-samy-deepPurple text-samy-deepPurple hover:text-white px-4 py-2.5 rounded-xl font-bold text-xs transition flex items-center gap-1.5">
<i data-lucide="plus" class="w-4 h-4"></i> Elegir Pack
</button>
</div>
</div>
</div>
</div>
</section>
<!-- About Section: Puerto Montt con amor -->
<section id="nosotras" class="py-16 bg-white">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="bg-gradient-to-r from-samy-purple/30 via-samy-lightpink to-samy-pink/30 rounded-3xl p-8 lg:p-12 border border-samy-pink/30 grid grid-cols-1 lg:grid-cols-2 gap-8 items-center">

<div class="space-y-4 text-center lg:text-left">
<span class="bg-white text-samy-deepPurple px-3.5 py-1 rounded-full text-xs font-bold uppercase tracking-wider shadow-sm">
📍 Hecho en el Sur de Chile
</span>
<h2 class="text-3xl sm:text-4xl font-fun text-gray-800">De Puerto Montt con Amor 💕</h2>
<p class="text-gray-600 text-sm sm:text-base leading-relaxed">
En <strong>Samy Imanes</strong> nos apasiona convertir tus recuerdos digitales en objetos tangibles llenos de significado. Todos nuestros imanes de <strong>5 cm x 5 cm</strong> se cortan e imprimen cuidadosamente en la ciudad de <strong>Puerto Montt, Región de Los Lagos</strong>.
</p>
<p class="text-gray-600 text-sm sm:text-base leading-relaxed">
Entregamos de forma presencial o con delivery en Puerto Montt y despachamos con amor a todas las ciudades y regiones de Chile por Starken, Chilexpress o Correos.
</p>

<div class="pt-2 flex flex-wrap gap-3 justify-center lg:justify-start">
<span class="bg-white/80 px-3 py-1.5 rounded-xl text-xs font-semibold text-gray-700 shadow-xs">📍 Puerto Montt</span>
<span class="bg-white/80 px-3 py-1.5 rounded-xl text-xs font-semibold text-gray-700 shadow-xs">🚚 Envíos a todo Chile</span>
<span class="bg-white/80 px-3 py-1.5 rounded-xl text-xs font-semibold text-gray-700 shadow-xs">📷 @samy_imanes</span>
</div>
</div>
<div class="flex justify-center">
<div class="relative max-w-sm">
<img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?auto=format&fit=crop&w=600&q=80" alt="Samy Imanes Puerto Montt" class="rounded-3xl shadow-xl border-4 border-white transform hover:rotate-1 transition duration-300">
<div class="absolute -bottom-4 -right-4 bg-white p-3 rounded-2xl shadow-lg border border-samy-pink flex items-center gap-2">
<span class="text-2xl">🇨🇱</span>
<div>
<p class="text-xs font-bold text-gray-800">Emprendimiento Chileno</p>
<p class="text-[10px] text-gray-500">Región de Los Lagos</p>
</div>
</div>
</div>
</div>
</div>
</div>
</section>
<!-- FAQ Section -->
<section id="faq" class="py-16 bg-samy-purple/15">
<div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="text-center mb-10">
<span class="bg-samy-purple text-samy-deepPurple px-4 py-1.5 rounded-full text-xs font-bold uppercase tracking-wider">Dudas Frecuentes</span>
<h2 class="text-3xl sm:text-4xl font-fun text-gray-800 mt-2">Preguntas Frecuentes</h2>
</div>
<div class="space-y-4">

<!-- FAQ Item 1 -->
<div class="bg-white rounded-2xl p-5 border border-samy-pink/20 shadow-xs cursor-pointer" onclick="toggleFaq(1)">
<div class="flex justify-between items-center">
<h3 class="font-bold text-gray-800 text-sm sm:text-base">¿Cuál es la medida de los imanes?</h3>
<i data-lucide="chevron-down" id="faq-icon-1" class="w-5 h-5 text-samy-darkpink transition-transform"></i>
</div>
<p id="faq-ans-1" class="hidden text-gray-600 text-xs sm:text-sm mt-3 pt-3 border-t border-gray-100">
Todos nuestros imanes tienen la medida estándar perfecta de <strong>5 cm x 5 cm</strong>. Es un formato cuadrado idéntico al de las publicaciones de Instagram, ideal para hacer collages en superficies metálicas.
</p>
</div>
<!-- FAQ Item 2 -->
<div class="bg-white rounded-2xl p-5 border border-samy-pink/20 shadow-xs cursor-pointer" onclick="toggleFaq(2)">
<div class="flex justify-between items-center">
<h3 class="font-bold text-gray-800 text-sm sm:text-base">¿Cómo les envío mis fotos de 5x5 cm?</h3>
<i data-lucide="chevron-down" id="faq-icon-2" class="w-5 h-5 text-samy-darkpink transition-transform"></i>
</div>
<p id="faq-ans-2" class="hidden text-gray-600 text-xs sm:text-sm mt-3 pt-3 border-t border-gray-100">
Una vez que agregues tu pack al carrito y presiones "Pedir por WhatsApp Directo", se abrirá nuestro chat en WhatsApp. Por ahí nos envías tus fotos elegidas directamente desde tu celular. Nosotras las encuadramos a 5x5 cm.
</p>
</div>
<!-- FAQ Item 3 -->
<div class="bg-white rounded-2xl p-5 border border-samy-pink/20 shadow-xs cursor-pointer" onclick="toggleFaq(3)">
<div class="flex justify-between items-center">
<h3 class="font-bold text-gray-800 text-sm sm:text-base">¿Tienen entregas en Puerto Montt y envíos?</h3>
<i data-lucide="chevron-down" id="faq-icon-3" class="w-5 h-5 text-samy-darkpink transition-transform"></i>
</div>
<p id="faq-ans-3" class="hidden text-gray-600 text-xs sm:text-sm mt-3 pt-3 border-t border-gray-100">
¡Sí! Entregamos en Puerto Montt de forma coordinada y realizamos envíos a todo Chile a través de Starken, Chilexpress o Correos de Chile.
</p>
</div>
<!-- FAQ Item 4 -->
<div class="bg-white rounded-2xl p-5 border border-samy-pink/20 shadow-xs cursor-pointer" onclick="toggleFaq(4)">
<div class="flex justify-between items-center">
<h3 class="font-bold text-gray-800 text-sm sm:text-base">¿El imán cubre toda la parte trasera?</h3>
<i data-lucide="chevron-down" id="faq-icon-4" class="w-5 h-5 text-samy-darkpink transition-transform"></i>
</div>
<p id="faq-ans-4" class="hidden text-gray-600 text-xs sm:text-sm mt-3 pt-3 border-t border-gray-100">
Absolutamente. Toda la superficie trasera de 5x5 cm es lámina imantada de primera calidad, asegurando que quede firme sin caerse del refrigerador.
</p>
</div>
</div>
</div>
</section>
<!-- Cart Modal Drawer -->
<div id="cart-backdrop" class="fixed inset-0 bg-black/40 backdrop-blur-xs z-50 hidden transition-opacity" onclick="toggleCart()"></div>

<div id="cart-drawer" class="fixed top-0 right-0 h-full w-full sm:w-96 bg-white z-50 shadow-2xl transform translate-x-full transition-transform duration-300 flex flex-col">

<!-- Cart Header -->
<div class="p-5 border-b border-gray-100 flex items-center justify-between bg-samy-lightpink/60">
<div class="flex items-center gap-2">
<i data-lucide="shopping-bag" class="w-5 h-5 text-samy-darkpink"></i>
<h3 class="font-fun text-2xl text-gray-800">Tu Carrito de Packs</h3>
</div>
<button onclick="toggleCart()" class="p-2 rounded-full hover:bg-gray-200 text-gray-500 transition">
<i data-lucide="x" class="w-5 h-5"></i>
</button>
</div>
<!-- Cart Items List -->
<div id="cart-items-list" class="flex-1 overflow-y-auto p-5 space-y-4 custom-scrollbar">
<!-- Items injected by JS -->
</div>
<!-- Cart Footer -->
<div class="p-5 border-t border-gray-100 bg-gray-50 space-y-4">
<div class="space-y-1.5 text-sm">
<div class="flex justify-between text-gray-600">
<span>Subtotal</span>
<span id="cart-subtotal-text" class="font-bold">$0</span>
</div>
<div class="flex justify-between text-gray-600 text-xs">
<span>Ubicación base</span>
<span class="text-samy-darkpink font-semibold">Puerto Montt, Los Lagos</span>
</div>
<div class="flex justify-between text-lg font-bold text-gray-800 pt-2 border-t border-gray-200">
<span>Total Final</span>
<span id="cart-total-text" class="text-samy-darkpink">$0</span>
</div>
</div>
<!-- Checkout Button -->
<button onclick="checkoutWhatsApp()" class="w-full bg-emerald-500 hover:bg-emerald-600 text-white font-bold py-3.5 rounded-2xl shadow-lg transition flex items-center justify-center gap-2 text-sm">
<i data-lucide="message-circle" class="w-5 h-5"></i>
Pedir por WhatsApp Directo
</button>
<p class="text-[11px] text-gray-500 text-center">Se abrirá WhatsApp con el resumen listo para adjuntar tus fotos de 5x5 cm.</p>
</div>
</div>
<!-- Toast Notification -->
<div id="toast" class="fixed bottom-6 right-6 z-50 transform translate-y-20 opacity-0 transition-all duration-300 bg-gray-900 text-white px-5 py-3.5 rounded-2xl shadow-2xl flex items-center gap-3 border border-gray-700">
<div class="w-8 h-8 rounded-full bg-samy-darkpink flex items-center justify-center text-white font-bold">
✓
</div>
<div>
<p id="toast-title" class="font-bold text-sm">¡Agregado!</p>
<p id="toast-msg" class="text-xs text-gray-300">Tu pack está en el carrito.</p>
</div>
</div>
<!-- Footer -->
<footer class="bg-gray-900 text-white mt-auto pt-12 pb-8">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="grid grid-cols-1 md:grid-cols-3 gap-8 pb-8 border-b border-gray-800">

<!-- Column 1: Info -->
<div class="space-y-3">
<div class="flex items-center gap-2">
<span class="text-2xl">🧲</span>
<span class="font-fun text-2xl text-samy-pink">Samy Imanes</span>
</div>
<p class="text-xs text-gray-400 leading-relaxed">
Fotografías imantadas cuadradas de 5 cm x 5 cm elaboradas en Puerto Montt, Región de Los Lagos, Chile.
</p>
<p class="text-xs text-samy-pink font-semibold">📍 Puerto Montt, Chile</p>
</div>
<!-- Column 2: Quick Links -->
<div>
<h4 class="font-bold text-sm text-samy-pink mb-3">Packs de Imanes 5x5 cm</h4>
<ul class="space-y-2 text-xs text-gray-400">
<li>Pack 6 imanes — $9.990</li>
<li>Pack 9 imanes — $13.990</li>
<li>Pack 12 imanes — $16.990 (Más vendido)</li>
<li>Pack 18 imanes — $24.990</li>
<li>Pack 24 imanes — $32.990 (Mejor valor)</li>
</ul>
</div>
<!-- Column 3: Instagram & Social -->
<div>
<h4 class="font-bold text-sm text-samy-pink mb-3">Redes Sociales</h4>
<a href="https://www.instagram.com/samy_imanes/" target="_blank" class="inline-flex items-center gap-2 bg-gradient-to-r from-purple-600 to-pink-600 px-4 py-2.5 rounded-xl text-xs font-bold hover:opacity-90 transition">
<i data-lucide="instagram" class="w-4 h-4"></i>
@samy_imanes en Instagram
</a>
<p class="text-[11px] text-gray-500 mt-3">¡Síguenos en Instagram para ver fotos de nuestros trabajos entregados!</p>
</div>
</div>
<div class="pt-6 text-center text-xs text-gray-500">
<p>&copy; 2026 Samy Imanes • Puerto Montt, Chile. Todos los derechos reservados.</p>
</div>
</div>
</footer>
<!-- Application Logic Script -->
<script>
// Official Packs Price Matrix
const PACK_PRICES = {
6: 6990,
9: 12990,
12: 16990,
18: 24990,
24: 32990
};
// State Management
let cart = [];
let simCurrentPhoto = 'https://images.unsplash.com/photo-1511895426328-dc8714191300?auto=format&fit=crop&w=500&q=80';
// Initialize Icons & Events
document.addEventListener('DOMContentLoaded', () => {
lucide.createIcons();
updateSimPack();
});
// Format Money to CLP Format
function formatCLP(amount) {
return '$' + amount.toLocaleString('es-CL');
}
// Simulator Logic
function updateSimPack() {
const count = parseInt(document.getElementById('sim-pack-select').value);
const price = PACK_PRICES[count];
document.getElementById('sim-price-tag').innerText = formatCLP(price);
}
function handleImageUpload(e) {
const file = e.target.files[0];
if (file) {
const reader = new FileReader();
reader.onload = function(evt) {
simCurrentPhoto = evt.target.result;
document.getElementById('sim-preview-img').src = simCurrentPhoto;
}
reader.readAsDataURL(file);
}
}
function setSamplePhoto(url) {
simCurrentPhoto = url;
document.getElementById('sim-preview-img').src = url;
}
function updateSimText() {
const val = document.getElementById('sim-text-input').value.trim();
const overlay = document.getElementById('sim-text-overlay');
if (val) {
overlay.innerText = val;
overlay.classList.remove('hidden');
} else {
overlay.classList.add('hidden');
}
}
function addSimulatedPackToCart() {
const count = parseInt(document.getElementById('sim-pack-select').value);
const price = PACK_PRICES[count];
const text = document.getElementById('sim-text-input').value.trim();
const item = {
id: 'custom-' + Date.now(),
name: `Pack ${count} Imanes 5x5 cm`,
count: count,
price: price,
customText: text || null,
image: simCurrentPhoto,
qty: 1
};
cart.push(item);
updateCartUI();
showToast("Pack Agregado", `Agregaste el Pack de ${count} imanes 5x5 cm.`);
toggleCart();
}
// Add Standard Catalog Pack to Cart
function addPackToCart(count, price) {
const existing = cart.find(i => i.count === count && !i.customText);
if (existing) {
existing.qty += 1;
} else {
cart.push({
id: 'pack-' + count + '-' + Date.now(),
name: `Pack ${count} Imanes 5x5 cm`,
count: count,
price: price,
customText: null,
image: 'https://images.unsplash.com/photo-1511895426328-dc8714191300?auto=format&fit=crop&w=400&q=80',
qty: 1
});
}
updateCartUI();
showToast("Pack Guardado", `Se agregó el Pack de ${count} imanes al carrito.`);
}
function updateCartQty(id, delta) {
const idx = cart.findIndex(i => i.id === id);
if (idx !== -1) {
cart[idx].qty += delta;
if (cart[idx].qty <= 0) {
cart.splice(idx, 1);
}
}
updateCartUI();
}
function updateCartUI() {
const badge = document.getElementById('cart-badge');
const totalItems = cart.reduce((sum, item) => sum + item.qty, 0);
badge.innerText = totalItems;
const container = document.getElementById('cart-items-list');
container.innerHTML = '';
if (cart.length === 0) {
container.innerHTML = `
<div class="text-center py-12 text-gray-400 space-y-3">
<i data-lucide="shopping-bag" class="w-12 h-12 mx-auto stroke-1 text-samy-pink"></i>
<p class="text-xs">Tu carrito está vacío.</p>
</div>
`;
} else {
let subtotal = 0;
cart.forEach(item => {
const itemTotal = item.price * item.qty;
subtotal += itemTotal;
const el = document.createElement('div');
el.className = "flex gap-3 bg-samy-lightpink/50 p-3 rounded-2xl border border-samy-pink/20 items-center";
el.innerHTML = `
<img src="${item.image}" alt="Imán 5x5" class="w-12 h-12 object-cover rounded-xl border border-white">
<div class="flex-1 min-w-0">
<h4 class="font-bold text-xs text-gray-800 truncate">${item.name}</h4>
<p class="text-[10px] text-gray-500">Medida: 5cm x 5cm</p>
${item.customText ? `<p class="text-[10px] text-samy-darkpink font-semibold truncate">"${item.customText}"</p>` : ''}
<p class="text-xs font-bold text-samy-darkpink mt-0.5">${formatCLP(item.price)}</p>
</div>
<div class="flex items-center gap-1.5 bg-white rounded-xl p-1 border border-gray-200">
<button onclick="updateCartQty('${item.id}', -1)" class="w-5 h-5 flex items-center justify-center text-xs font-bold text-gray-600 hover:bg-gray-100 rounded-lg">-</button>
<span class="text-xs font-bold text-gray-800 px-1">${item.qty}</span>
<button onclick="updateCartQty('${item.id}', 1)" class="w-5 h-5 flex items-center justify-center text-xs font-bold text-gray-600 hover:bg-gray-100 rounded-lg">+</button>
</div>
`;
container.appendChild(el);
});
document.getElementById('cart-subtotal-text').innerText = formatCLP(subtotal);
document.getElementById('cart-total-text').innerText = formatCLP(subtotal);
}
lucide.createIcons();
}
function toggleCart() {
const drawer = document.getElementById('cart-drawer');
const backdrop = document.getElementById('cart-backdrop');
drawer.classList.toggle('translate-x-full');
backdrop.classList.toggle('hidden');
}
function toggleMobileMenu() {
document.getElementById('mobile-menu').classList.toggle('hidden');
}
function toggleFaq(id) {
const ans = document.getElementById(`faq-ans-${id}`);
const icon = document.getElementById(`faq-icon-${id}`);
ans.classList.toggle('hidden');
icon.classList.toggle('rotate-180');
}
function showToast(title, msg) {
const toast = document.getElementById('toast');
document.getElementById('toast-title').innerText = title;
document.getElementById('toast-msg').innerText = msg;
toast.classList.remove('translate-y-20', 'opacity-0');
toast.classList.add('translate-y-0', 'opacity-100');
setTimeout(() => {
toast.classList.remove('translate-y-0', 'opacity-100');
toast.classList.add('translate-y-20', 'opacity-0');
}, 3000);
}
// WhatsApp Checkout Direct Link
function checkoutWhatsApp() {
if (cart.length === 0) {
showToast("Carrito Vacío", "Añade al menos un pack de imanes para continuar.");
return;
}
let text = "¡Hola Samy Imanes! 🧲✨ Quisiera coordinar el siguiente pedido desde la página web:\n\n";
let total = 0;
cart.forEach((item, index) => {
const itemTotal = item.price * item.qty;
total += itemTotal;
text += `${index + 1}. *${item.name}* (5x5 cm) x${item.qty}\n`;
if (item.customText) {
text += `   ↳ Texto/Nota: "${item.customText}"\n`;
}
text += `   ↳ Precio: ${formatCLP(itemTotal)}\n\n`;
});
text += `*Total a pagar:* ${formatCLP(total)}\n`;
text += `*Ubicación:* Puerto Montt / Envío a Regiones\n\n`;
text += "Quedo atento(a) para enviar las fotografías por este chat y acordar la entrega/envío. ¡Muchas gracias!";
const encodedText = encodeURIComponent(text);
const whatsappUrl = `https://wa.me/56912345678?text=${encodedText}`;
window.open(whatsappUrl, '_blank');
}
</script>

<a href="https://wa.me/56920563897?text=Hola%20Samy%20Imanes%2C%20quiero%20hacer%20una%20consulta" target="_blank" rel="noopener noreferrer" aria-label="Contactar por WhatsApp" style="position:fixed;right:20px;bottom:20px;z-index:9999;background:#25D366;color:white;width:58px;height:58px;border-radius:50%;display:flex;align-items:center;justify-content:center;box-shadow:0 6px 20px rgba(0,0,0,.25);text-decoration:none;font-size:30px;font-weight:700;">◉</a>
</body>
</html>
