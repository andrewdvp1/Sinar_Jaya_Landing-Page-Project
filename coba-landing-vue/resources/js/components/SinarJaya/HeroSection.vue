<template>
  <div class="relative min-h-screen bg-[#1A1A1A] flex flex-col justify-between text-white overflow-hidden">
    
    <div class="absolute inset-0 z-0">
      <img src="https://images.unsplash.com/photo-1617038260897-41a1f14a8ca0?w=1600&auto=format&fit=crop&q=80" alt="Sinar Jaya Background" class="w-full h-full object-cover opacity-25 scale-105 transition-transform duration-1000">
      <div class="absolute inset-0 bg-black/40"></div>
      <div class="absolute inset-0 bg-gradient-to-b from-black/60 via-transparent to-black/40"></div>
    </div>

    <nav class="relative z-10 w-full max-w-7xl mx-auto px-6 sm:px-12 py-6 flex items-center justify-between border-b border-white/5 backdrop-blur-md bg-black/10">
      <div class="font-serif text-2xl lg:text-3xl tracking-widest text-[#D4AF37] font-bold uppercase">
        Sinar Jaya
      </div>
      
      <div class="hidden md:flex items-center gap-10 text-[11px] uppercase tracking-[0.25em] font-medium text-zinc-300">
        <a href="#koleksi" class="hover:text-[#D4AF37] transition duration-300">Koleksi</a>
        <a href="#keunggulan" class="hover:text-[#D4AF37] transition duration-300">Keunggulan</a>
        <a href="#tentang-kami" class="hover:text-[#D4AF37] transition duration-300">Tentang Kami</a>
        <a href="#hubungi-kami" class="hover:text-[#D4AF37] transition duration-300">Hubungi Kami</a>
      </div>

      <a :href="waLink" target="_blank" class="bg-transparent hover:bg-[#D4AF37] border border-[#D4AF37] text-[#D4AF37] hover:text-black font-semibold uppercase tracking-[0.15em] text-[10px] px-6 py-2.5 transition-all duration-300">
        RESERVASI WA
      </a>
    </nav>

    <div class="relative z-10 flex-grow flex items-center max-w-4xl mx-auto px-6 text-center py-20">
      <div class="space-y-6">
        <span class="text-[#D4AF37] uppercase tracking-[0.4em] text-[10px] sm:text-[11px] font-bold block">
          THE LUMINOUS HERITAGE
        </span>
        
        <h1 class="font-serif text-3xl md:text-5xl lg:text-6xl font-light tracking-tight leading-[1.2] text-white max-w-3xl mx-auto">
          Kilau Abadi, Investasi Terpercaya: Sinar Jaya Menghadirkan Kemewahan yang Nyata.
        </h1>
        
        <p class="text-zinc-200 max-w-2xl mx-auto text-sm font-light leading-relaxed tracking-wide">
          Keindahan emas yang tak lekang oleh waktu bersanding dengan kepastian nilai investasi. Temukan koleksi eksklusif kami yang telah dipercaya selama lintas generasi.
        </p>

        <div class="flex flex-col sm:flex-row items-center justify-center gap-4 pt-6">
          <a href="#koleksi" class="w-full sm:w-auto bg-[#D4AF37] hover:bg-[#bfa032] text-black font-bold uppercase tracking-[0.2em] text-[11px] px-8 py-4 transition-all duration-300 shadow-lg shadow-black/20">
            EKSPLOR KOLEKSI
          </a>
          <a :href="waLink" target="_blank" class="w-full sm:w-auto border border-zinc-400 hover:border-white hover:bg-white/10 text-white font-semibold uppercase tracking-[0.2em] text-[11px] px-8 py-4 transition-all duration-300">
            HARGA HARI INI
          </a>
        </div>
      </div>
    </div>

    <div class="relative z-10 w-full bg-[#FDFBF7] py-6 border-t border-zinc-800">
      <div class="max-w-6xl mx-auto px-6 grid grid-cols-2 md:grid-cols-4 gap-6 text-center">
        
        <div class="flex flex-col items-center justify-center gap-2 text-[#1A1A1A] text-[10px] uppercase tracking-[0.15em] font-semibold">
          <Icon icon="lucide:award" class="text-[#D4AF37] text-2xl" />
          <span>JAMINAN EMAS ASLI</span>
        </div>
        
        <div class="flex flex-col items-center justify-center gap-2 text-[#1A1A1A] text-[10px] uppercase tracking-[0.15em] font-semibold">
          <Icon icon="lucide:refresh-cw" class="text-[#D4AF37] text-2xl" />
          <span>BUYBACK GUARANTEE</span>
        </div>
        
        <div class="flex flex-col items-center justify-center gap-2 text-[#1A1A1A] text-[10px] uppercase tracking-[0.15em] font-semibold">
          <Icon icon="lucide:file-check" class="text-[#D4AF37] text-2xl" />
          <span>SERTIFIKAT LENGKAP</span>
        </div>
        
        <div class="flex flex-col items-center justify-center gap-2 text-[#1A1A1A] text-[10px] uppercase tracking-[0.15em] font-semibold">
          <Icon icon="lucide:map-pin" class="text-[#D4AF37] text-2xl" />
          <span>TOKO FISIK RESMI</span>
        </div>

      </div>
    </div>

  </div>
</template>

<script setup>
import { computed } from 'vue'
import { Icon } from '@iconify/vue' // IMPORT COMPONENT ICONIFY

const phoneNumber = '628123456789'
const defaultMessage = 'Halo Sinar Jaya, saya ingin tanya seputar koleksi perhiasannya.'
const waLink = computed(() => `https://wa.me/${phoneNumber}?text=${encodeURIComponent(defaultMessage)}`)
</script>