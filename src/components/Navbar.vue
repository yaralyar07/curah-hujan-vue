<template>
  <header class="sticky top-0 z-50 w-full bg-white/95 backdrop-blur-sm border-b border-gray-100 shadow-sm transition-all duration-300">
    
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center h-20">
        
        <div class="flex-shrink-0 flex items-center cursor-pointer">
          <div class="w-10 h-10 bg-blue-500 rounded-lg flex items-center justify-center mr-3 text-white">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 15a4 4 0 004 4h9a5 5 0 10-.1-9.999 5.002 5.002 0 10-9.78 2.096A4.001 4.001 0 003 15z" />
            </svg>
          </div>
          <span class="font-bold text-xl text-gray-800 tracking-tight">Cuaca<span class="text-blue-500">Kita</span></span>
        </div>

        <nav class="hidden md:flex items-center space-x-8">
          <a 
            v-for="(item, index) in navLinks" 
            :key="index" 
            href="#" 
            class="text-sm font-medium text-gray-500 hover:text-blue-600 transition-colors duration-200"
          >
            {{ item }}
          </a>

          <button class="bg-blue-600 text-white text-sm font-medium px-5 py-2.5 rounded-full shadow-lg shadow-blue-500/30 hover:bg-blue-700 hover:shadow-blue-500/40 transition-all duration-300 transform hover:-translate-y-0.5">
            Contact Center
          </button>
        </nav>

        <div class="md:hidden flex items-center">
          <button class="text-gray-500 hover:text-gray-700 focus:outline-none">
            <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            </svg>
          </button>
        </div>

      </div>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue';

// Data Menu (Tanpa Contact Center karena dipisah jadi tombol)
const navLinks = ref([
  'Profil',
  'Cuaca',
  'Iklim',
  'Kualitas Udara'
]);
</script>