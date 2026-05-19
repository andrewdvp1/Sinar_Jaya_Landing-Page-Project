<template>
  <div class="relative min-h-[90vh] bg-[#1A1A1A] flex flex-col justify-between text-white overflow-hidden">
    
    <div class="absolute inset-0 z-0">
      <img src="https://images.unsplash.com/photo-1617038260897-41a1f14a8ca0?w=1600&auto=format&fit=crop&q=80" alt="Sinar Jaya Background" class="w-full h-full object-cover opacity-35 scale-100">
      <div class="absolute inset-0 bg-gradient-to-b from-black/50 via-transparent to-[#FDFBF7]/5"></div>
    </div>

    <nav class="relative z-10 w-full max-w-6xl mx-auto px-6 py-4 flex items-center justify-between border-b border-white/10 backdrop-blur-sm bg-black/5">
      <div class="font-serif text-xl lg:text-2xl tracking-wide text-[#D4AF37] font-bold">
        Sinar Jaya
      </div>
      
      <div class="hidden md:flex items-center gap-6 text-[11px] uppercase tracking-[0.2em] font-medium text-gray-300">
        <a href="#koleksi" class="hover:text-[#D4AF37] transition">Koleksi</a>
        <a href="#keunggulan" class="hover:text-[#D4AF37] transition">Keunggulan</a>
        <a href="#tentang-kami" class="hover:text-[#D4AF37] transition">Tentang Kami</a>
        <a href="#hubungi-kami" class="hover:text-[#D4AF37] transition">Hubungi Kami</a>
      </div>

      <a :href="waLink" target="_blank" class="bg-black hover:bg-zinc-900 border border-[#D4AF37] text-[#D4AF37] font-medium uppercase tracking-wider text-[10px] px-4 py-2 transition">
        RESERVASI WA
      </a>
    </nav>

    <div class="relative z-10 flex-grow flex items-center max-w-3xl mx-auto px-6 text-center py-12">
      <div class="space-y-4">
        <span class="text-[#D4AF37] uppercase tracking-[0.3em] text-[10px] font-bold block">
          THE LUMINOUS HERITAGE
        </span>
        
        <h1 class="font-serif text-2xl md:text-4xl font-normal tracking-wide leading-snug text-white">
          Kilau Abadi, Investasi Terpercaya: Sinar Jaya Menghadirkan Kemewahan yang Nyata.
        </h1>
        
        <p class="text-gray-300 max-w-xl mx-auto text-xs font-light leading-relaxed opacity-90">
          Keindahan emas yang tak lekang oleh waktu bersanding dengan kepastian nilai investasi. Temukan koleksi eksklusif kami yang telah dipercaya selama lintas generasi.
        </p>

        <div class="flex items-center justify-center gap-3 pt-2">
          <a href="#koleksi" class="bg-[#D4AF37] hover:bg-[#bfa032] text-black font-semibold uppercase tracking-widest text-[10px] px-6 py-3 transition">
            EKSPLOR KOLEKSI
          </a>
          <a :href="waLink" target="_blank" class="border border-white/40 hover:border-white hover:bg-white/10 text-white font-medium uppercase tracking-widest text-[10px] px-6 py-3 transition">
            HARGA HARI INI
          </a>
        </div>
      </div>
    </div>

    <div class="relative z-10 w-full bg-[#F5F2EA] py-4 border-t border-b border-[#EAE5D9]/50">
      <div class="max-w-5xl mx-auto px-4 grid grid-cols-2 md:grid-cols-4 gap-4 text-center">
        <div class="flex flex-col items-center justify-center gap-1 text-[#1A1A1A] text-[10px] uppercase tracking-wider font-medium">
          <span class="text-[#D4AF37] text-sm">🏆</span> JAMINAN EMAS ASLI
        </div>
        <div class="flex flex-col items-center justify-center gap-1 text-[#1A1A1A] text-[10px] uppercase tracking-wider font-medium">
          <span class="text-[#D4AF37] text-sm">🔄</span> TERIMA JUAL KEMBALI (BUYBACK)
        </div>
        <div class="flex flex-col items-center justify-center gap-1 text-[#1A1A1A] text-[10px] uppercase tracking-wider font-medium">
          <span class="text-[#D4AF37] text-sm">📜</span> SERTIFIKAT FULL LENGKAP
        </div>
        <div class="flex flex-col items-center justify-center gap-1 text-[#1A1A1A] text-[10px] uppercase tracking-wider font-medium">
          <span class="text-[#D4AF37] text-sm">📍</span> TOKO FISIK TERVERIFIKASI
        </div>
      </div>
    </div>

  </div>
</template>

<script setup>
import { computed } from 'vue'
const phoneNumber = '628123456789'
const defaultMessage = 'Halo Sinar Jaya, saya ingin tanya seputar koleksi perhiasannya.'
const waLink = computed(() => `https://wa.me/${phoneNumber}?text=${encodeURIComponent(defaultMessage)}`)
</script>