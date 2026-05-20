<template>
  <section id="tentang-kami" class="bg-[#FDFBF7] py-20 px-6 border-t border-[#EAE5D9]/30">
    <div class="max-w-5xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-12 md:gap-16 items-center">
      
      <div class="relative w-full max-w-sm justify-self-center md:justify-self-start group">
        <div class="absolute -inset-3 border border-[#D4AF37]/30 translate-x-2 translate-y-2 transition-transform duration-500 group-hover:translate-x-0 group-hover:translate-y-0 hidden sm:block"></div>
        
        <div class="w-full h-[440px] bg-zinc-100 overflow-hidden relative border border-[#EAE5D9] shadow-md z-10">
          
          <div 
            v-for="(img, index) in images" 
            :key="index"
            class="absolute inset-0 w-full h-full transition-opacity duration-1000 ease-in-out"
            :class="currentIndex === index ? 'opacity-100 z-10' : 'opacity-0 z-0'"
          >
            <img 
              :src="img" 
              alt="Koleksi Sinar Jaya" 
              class="w-full h-full object-cover transition-transform duration-700 ease-out group-hover:scale-105"
            >
          </div>

          <button 
            @click="prevSlide" 
            class="absolute left-3 top-1/2 -translate-y-1/2 bg-black/40 hover:bg-black/70 text-white p-2 rounded-full z-30 opacity-0 group-hover:opacity-100 transition-opacity duration-300 backdrop-blur-sm"
          >
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg>
          </button>

          <button 
            @click= "nextSlide" 
            class="absolute right-3 top-1/2 -translate-y-1/2 bg-black/40 hover:bg-black/70 text-white p-2 rounded-full z-30 opacity-0 group-hover:opacity-100 transition-opacity duration-300 backdrop-blur-sm"
          >
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="m9 18 6-6-6-6"/></svg>
          </button>

          <div class="absolute bottom-4 left-4 flex gap-1.5 z-30">
            <button 
              v-for="(_, index) in images" 
              :key="index"
              @click="goToSlide(index)"
              class="h-1 transition-all duration-300 rounded-full"
              :class="currentIndex === index ? 'w-6 bg-[#D4AF37]' : 'w-1.5 bg-white/60'"
            ></button>
          </div>
          
          <div class="absolute bottom-0 right-0 bg-[#1A1A1A] text-white py-4 px-6 text-center min-w-[110px] shadow-xl z-30">
            <span class="block text-2xl font-serif text-[#D4AF37] font-normal tracking-wide">40+</span>
            <span class="block text-[8px] uppercase tracking-[0.2em] text-zinc-400 mt-1 font-medium">Tahun Melayani</span>
          </div>
        </div>
      </div>

      <div class="space-y-6 text-left z-10">
        <div class="space-y-2">
          <span class="text-[#D4AF37] uppercase tracking-[0.4em] text-[10px] font-bold block">
            WARISAN KEINDAHAN
          </span>
          <h2 class="font-serif text-2xl md:text-3xl lg:text-4xl font-light text-[#1A1A1A] tracking-wide leading-tight">
            Dedikasi Terhadap Keaslian & Kepercayaan
          </h2>
        </div>
        
        <div class="space-y-4 text-zinc-600 font-light leading-relaxed text-xs sm:text-[13px]">
          <p>
            Toko Mas Sinar Jaya telah berdiri selama puluhan tahun sebagai simbol kejujuran di industri perhiasan. Kami memahami bahwa setiap emas yang Anda beli adalah bentuk kerja keras dan masa depan Anda.
          </p>
          <p>
            Dengan komitmen <span class="italic text-[#1A1A1A] font-normal">"Information-Driven Luxury"</span>, kami menyediakan edukasi lengkap bagi setiap pelanggan agar investasi Anda tetap aman dan bernilai tinggi secara jangka panjang.
          </p>
        </div>

        <div class="border border-[#D4AF37]/40 bg-[#1A1A1A] p-4 rounded-none shadow-sm">
          <p class="font-serif text-xs sm:text-[13px] italic text-[#D4AF37] leading-relaxed">
            "Kilau abadi bukan hanya pada perhiasannya, tapi pada kepercayaan pelanggan yang selalu kami jaga."
          </p>
        </div>

        <div class="pt-2">
          <a href="#hubungi-kami" class="inline-flex items-center gap-2 text-[10px] uppercase tracking-[0.2em] font-semibold text-[#1A1A1A] hover:text-[#D4AF37] transition group">
            <span>Selengkapnya Tentang Kami</span>
            <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" class="transition-transform duration-300 group-hover:translate-x-1.5">
              <path d="M5 12h14M12 5l7 7-7 7"/>
            </svg>
          </a>
        </div>
      </div>

    </div>
  </section>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

// 1. Array Kumpulan Gambar Mewah (Bisa Lu Ganti/Tambah Sesuka Hati)
const images = ref([
  'https://images.unsplash.com/photo-1630019852942-f89202989a59?w=600&auto=format&fit=crop&q=80', // Anting Daun Hijau
  'https://images.unsplash.com/photo-1599643478518-a784e5dc4c8f?w=600&auto=format&fit=crop&q=80', // Cincin Berlian Luxury
  'https://images.unsplash.com/photo-1602751584552-8ba73aad10e1?w=600&auto=format&fit=crop&q=80'  // Kalung Emas Premium
])

const currentIndex = ref(0)
let timer = null

// 2. Fungsi Navigasi Slider
const nextSlide = () => {
  currentIndex.value = (currentIndex.value + 1) % images.value.length
}

const prevSlide = () => {
  currentIndex.value = (currentIndex.value - 1 + images.value.length) % images.value.length
}

const goToSlide = (index) => {
  currentIndex.value = index
}

// 3. Efek Auto Play (Berpindah otomatis setiap 4 detik)
onMounted(() => {
  timer = setInterval(nextSlide, 4000)
})

onUnmounted(() => {
  if (timer) clearInterval(timer)
})
</script>