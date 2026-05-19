<template>
  <div class="min-h-screen bg-[#FDFBF7] font-sans antialiased selection:bg-[#D4AF37] selection:text-white scroll-smooth">
    
    <HeroSection />

    <FeaturesSection />

    <CatalogSection />

    <AboutSection />

    <ContactFooterSection />

  </div>
</template>

<script setup>
// Sesuaikan jalur import ini dengan folder tempat lu naruh 5 file SinarJaya kemarin
import HeroSection from '@/components/SinarJaya/HeroSection.vue'
import FeaturesSection from '@/components/SinarJaya/FeaturesSection.vue'
import CatalogSection from '@/components/SinarJaya/CatalogSection.vue'
import AboutSection from '@/components/SinarJaya/AboutSection.vue'
import ContactFooterSection from '@/components/SinarJaya/ContactFooterSection.vue'
</script>