<template>
  <div>
    <section id="hubungi-kami" class="bg-[#FDFBF7] py-20 px-6 border-t border-[#EAE5D9]/30">
      <div class="max-w-5xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-12 md:gap-16 items-center">
        
        <div class="space-y-6 text-left">
          <div class="space-y-2">
            <span class="text-[#D4AF37] uppercase tracking-[0.4em] text-[10px] font-bold block">
              KUNJUNGI KAMI
            </span>
            <h2 class="font-serif text-2xl md:text-3xl font-light text-[#1A1A1A] tracking-wide leading-tight">
              Pusat Keindahan di Jantung Jakarta
            </h2>
          </div>
          
          <p class="text-zinc-500 font-light text-xs sm:text-[13px] leading-relaxed">
            Temukan kami di kawasan legendaris perhiasan Jakarta untuk mendapatkan pelayanan konsultasi eksklusif dan melihat koleksi lengkap kami secara langsung.
          </p>

          <div class="space-y-4 pt-5 border-t border-[#EAE5D9]">
            <div class="flex items-start gap-3.5 group">
              <div class="text-[#D4AF37] mt-0.5 transition-transform duration-300 group-hover:scale-110">
                <Icon icon="lucide:map-pin" class="text-base" />
              </div>
              <div>
                <h4 class="font-serif text-sm font-normal text-[#1A1A1A] tracking-wide">Pusat Perhiasan Cikini Gold Center</h4>
                <p class="text-zinc-400 text-xs font-light mt-1 leading-relaxed">Lantai Dasar, Blok A No. 12-15, Jakarta Pusat, DKI Jakarta 10330</p>
              </div>
            </div>
            
            <div class="flex items-start gap-3.5 group">
              <div class="text-[#D4AF37] mt-0.5 transition-transform duration-300 group-hover:scale-110">
                <Icon icon="lucide:clock" class="text-base" />
              </div>
              <div>
                <h4 class="font-serif text-sm font-normal text-[#1A1A1A] tracking-wide">Jam Operasional</h4>
                <p class="text-zinc-400 text-xs font-light mt-1">Senin - Minggu: 10.00 - 18.00 WIB</p>
              </div>
            </div>
          </div>
        </div>

        <div class="relative w-full group">
          <div class="absolute -inset-3 border border-[#D4AF37]/20 translate-x-1.5 translate-y-1.5 transition-transform duration-500 group-hover:translate-x-0 group-hover:translate-y-0 hidden sm:block"></div>
          
          <div class="w-full h-64 md:h-80 bg-zinc-100 border border-[#EAE5D9] shadow-md overflow-hidden rounded-none relative z-10">
            <iframe 
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3966.4913251410114!2d106.8379435!3d-6.1987258!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e69f430b809a939%3A0x6b77242274b3adfd!2sCikini%20Gold%20Center!5e0!3m2!1sid!2sid!4v1716200000000!5m2!1sid!2sid" 
              class="w-full h-full border-0 grayscale opacity-90 hover:grayscale-0 transition-all duration-700 ease-out" 
              allowfullscreen="" 
              loading="lazy" 
              referrerpolicy="no-referrer-when-downgrade">
            </iframe>
          </div>
        </div>

      </div>
    </section>

    <footer class="bg-[#1A1A1A] text-white py-12 px-6 border-t border-white/5">
      <div class="max-w-5xl mx-auto flex flex-col md:flex-row justify-between items-center gap-6">
        
        <div class="text-center md:text-left space-y-1">
          <h3 class="font-serif text-xl tracking-[0.15em] text-[#D4AF37] font-light uppercase">Sinar Jaya</h3>
          <p class="text-[10px] tracking-wider text-zinc-500 font-light pt-0.5">
            © 2026 Toko Mas Sinar Jaya. Kilau Abadi, Investasi Terpercaya.
          </p>
        </div>

        <div class="flex flex-wrap justify-center gap-x-6 gap-y-2 text-[10px] tracking-[0.2em] text-zinc-400 font-light uppercase">
          <a href="#" class="relative hover:text-[#D4AF37] transition duration-300 after:absolute after:bottom-0 after:left-0 after:w-0 after:h-[1px] after:bg-[#D4AF37] after:transition-all hover:after:w-full pb-0.5">Kebijakan Privasi</a>
          <a href="#" class="relative hover:text-[#D4AF37] transition duration-300 after:absolute after:bottom-0 after:left-0 after:w-0 after:h-[1px] after:bg-[#D4AF37] after:transition-all hover:after:w-full pb-0.5">Syarat & Ketentuan</a>
          <a href="#" class="relative hover:text-[#D4AF37] transition duration-300 after:absolute after:bottom-0 after:left-0 after:w-0 after:h-[1px] after:bg-[#D4AF37] after:transition-all hover:after:w-full pb-0.5">Sertifikat OJK</a>
          <a href="#" class="relative hover:text-[#D4AF37] transition duration-300 after:absolute after:bottom-0 after:left-0 after:w-0 after:h-[1px] after:bg-[#D4AF37] after:transition-all hover:after:w-full pb-0.5">Bantuan</a>
        </div>

      </div>
    </footer>
  </div>
</template>

<script setup>
import { Icon } from '@iconify/vue'
</script>