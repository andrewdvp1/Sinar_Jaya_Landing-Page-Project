<template>
  <section id="koleksi" class="bg-[#FDFBF7] py-16 px-6">
    <div class="max-w-5xl mx-auto">
      
      <div class="text-center mb-12 space-y-2">
        <span class="text-[#D4AF37] uppercase tracking-[0.3em] text-[10px] font-bold block">
          PRODUK TERATAS
        </span>
        <h2 class="font-serif text-2xl md:text-3xl font-normal text-[#1A1A1A] tracking-wide">
          Koleksi Unggulan
        </h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        
        <div class="bg-white border border-[#EAE5D9] p-4 flex flex-col rounded-sm transition-all duration-300 hover:shadow-sm">
          <div class="aspect-[4/4] bg-gray-50 overflow-hidden mb-4 rounded-sm">
            <img src="https://images.unsplash.com/photo-1617038260897-41a1f14a8ca0?w=500&auto=format&fit=crop&q=80" alt="Necklace" class="w-full h-full object-cover">
          </div>
          <div class="text-center space-y-1">
            <span class="text-[#D4AF37] uppercase tracking-widest text-[9px] font-bold block">Necklace Collection</span>
            <h3 class="font-serif text-base font-normal text-[#1A1A1A]">Eternal Ribbon Gold Necklace</h3>
            <p class="text-gray-400 text-[11px] font-light leading-relaxed pt-1">Kemewahan 24k dengan detail ukiran artisan elegan.</p>
          </div>
        </div>

        <div class="bg-white border border-[#EAE5D9] p-4 flex flex-col rounded-sm transition-all duration-300 hover:shadow-sm">
          <div class="aspect-[4/4] bg-gray-50 overflow-hidden mb-4 rounded-sm">
            <img src="https://images.unsplash.com/photo-1617038260897-41a1f14a8ca0?w=500&auto=format&fit=crop&q=80" alt="Ring" class="w-full h-full object-cover">
          </div>
          <div class="text-center space-y-1">
            <span class="text-[#D4AF37] uppercase tracking-widest text-[9px] font-bold block">Ring Collection</span>
            <h3 class="font-serif text-base font-normal text-[#1A1A1A]">Majesty Diamond Ring</h3>
            <p class="text-gray-400 text-[11px] font-light leading-relaxed pt-1">Perpaduan emas putih dan berlian kualitas VVS.</p>
          </div>
        </div>

        <div class="bg-white border border-[#EAE5D9] p-4 flex flex-col rounded-sm transition-all duration-300 hover:shadow-sm">
          <div class="aspect-[4/4] bg-gray-50 overflow-hidden mb-4 rounded-sm">
            <img src="https://images.unsplash.com/photo-1617038260897-41a1f14a8ca0?w=500&auto=format&fit=crop&q=80" alt="Bangle" class="w-full h-full object-cover">
          </div>
          <div class="text-center space-y-1">
            <span class="text-[#D4AF37] uppercase tracking-widest text-[9px] font-bold block">Bracelet Collection</span>
            <h3 class="font-serif text-base font-normal text-[#1A1A1A]">Luminous Heritage Bangle</h3>
            <p class="text-gray-400 text-[11px] font-light leading-relaxed pt-1">Desain warisan budaya modern berkelas profesional.</p>
          </div>
        </div>

      </div>

      <div class="text-center mt-10">
        <a :href="waLink" target="_blank" class="inline-flex items-center justify-center bg-[#1A1A1A] hover:bg-black text-[#D4AF37] font-medium uppercase tracking-[0.15em] text-[10px] px-8 py-3 transition rounded-sm shadow-sm gap-2">
          LIHAT KOLEKSI LENGKAP DI WHATSAPP 💬
        </a>
      </div>

    </div>
  </section>
</template>

<script setup>
import { computed } from 'vue'
const phoneNumber = '628123456789'
const waLink = computed(() => `https://wa.me/${phoneNumber}?text=Halo%20Sinar%20Jaya%2C%20saya%20tertarik%20melihat%20katalog%20lengkapnya.`)
</script>