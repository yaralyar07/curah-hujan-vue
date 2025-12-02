<template>
  <section class="relative w-full h-screen flex flex-col justify-center items-center overflow-hidden">
    
    <div 
      class="absolute inset-0 z-0 bg-cover bg-center"
      style="background-image: url('https://images.unsplash.com/photo-1515694346937-94d85e41e6f0?q=80&w=2000&auto=format&fit=crop');" 
    >
      <div class="absolute inset-0 bg-blue-500/20 mix-blend-overlay"></div>
    </div>

    <div class="relative z-10 text-center px-4">
      
      <h1 class="text-white text-6xl md:text-8xl mb-12 pixel-font leading-tight drop-shadow-md">
        Curah<br>Hujan
      </h1>

      <button class="bg-white text-blue-900 font-semibold py-3 px-8 rounded-full shadow-lg hover:bg-gray-100 hover:scale-105 transition-all duration-300">
        Baca Selengkapnya
      </button>
      
    </div>
  </section>
</template>

<style scoped>
/* Implementasi font pixel khusus untuk komponen ini */
.pixel-font {
  font-family: 'Press Start 2P', cursive;
}
</style>