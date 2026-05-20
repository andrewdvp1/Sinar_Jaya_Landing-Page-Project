<template>
  <section id="keunggulan" class="bg-[#FDFBF7] py-20 px-6 border-b border-[#EAE5D9]/30">
    <div class="max-w-5xl mx-auto">
      
      <div class="text-center mb-16 space-y-3">
        <span class="text-[#D4AF37] uppercase tracking-[0.4em] text-[10px] sm:text-[11px] font-bold block">
          MENGAPA SINAR JAYA
        </span>
        <h2 class="font-serif text-3xl md:text-4xl font-light text-[#1A1A1A] tracking-wide">
          3 Keunggulan Utama
        </h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-8 items-stretch">
        
        <div class="bg-white border border-[#EAE5D9] p-8 flex flex-col items-center text-center rounded-sm transition-all duration-300 hover:shadow-md hover:border-[#D4AF37]/30 group">
          <div class="w-12 h-12 rounded-full border border-[#EAE5D9] group-hover:border-[#D4AF37]/50 flex items-center justify-center text-[#D4AF37] mb-5 bg-[#FDFBF7] transition-all duration-300">
            <Icon icon="lucide:shield-check" class="text-xl" />
          </div>
          <h3 class="font-serif text-xl font-normal text-[#1A1A1A] mb-3">Kualitas Terjamin</h3>
          <p class="text-zinc-500 text-xs sm:text-[13px] font-light leading-relaxed">
            Setiap karat emas kami disertai sertifikasi resmi dan standar kemurnian tertinggi untuk Anda.
          </p>
        </div>

        <div class="bg-[#1A1A1A] border border-[#1A1A1A] p-8 flex flex-col items-center text-center rounded-sm shadow-xl text-white transform md:-translate-y-2 transition-all duration-300">
          <div class="w-12 h-12 rounded-full border border-white/10 flex items-center justify-center text-[#D4AF37] mb-5 bg-white/5">
            <Icon icon="lucide:gem" class="text-xl" />
          </div>
          <h3 class="font-serif text-xl font-normal text-[#D4AF37] mb-3 tracking-wide">Desain Eksklusif</h3>
          <p class="text-zinc-300 text-xs sm:text-[13px] font-light leading-relaxed">
            Karya seni gabungan tradisi klasik dengan sentuhan modern prestisius yang membuat Anda bersinar.
          </p>
        </div>

        <div class="bg-white border border-[#EAE5D9] p-8 flex flex-col items-center text-center rounded-sm transition-all duration-300 hover:shadow-md hover:border-[#D4AF37]/30 group">
          <div class="w-12 h-12 rounded-full border border-[#EAE5D9] group-hover:border-[#D4AF37]/50 flex items-center justify-center text-[#D4AF37] mb-5 bg-[#FDFBF7] transition-all duration-300">
            <Icon icon="lucide:tag" class="text-xl" />
          </div>
          <h3 class="font-serif text-xl font-normal text-[#1A1A1A] mb-3">Harga Transparan</h3>
          <p class="text-zinc-500 text-xs sm:text-[13px] font-light leading-relaxed">
            Kepercayaan adalah fondasi kami. Dapatkan nilai emas real-time sesuai standar pasar global.
          </p>
        </div>

      </div>

    </div>
  </section>
</template>

<script setup>
import { Icon } from '@iconify/vue' // IMPORT ICONIFY
</script>