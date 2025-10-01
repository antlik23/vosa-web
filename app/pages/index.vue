<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section class="min-h-screen flex flex-col justify-center items-center text-white px-4">
      <div class="text-center max-w-4xl mx-auto">
        <!-- Royal Flush Logo -->
        <div class="mb-8">
          <img 
            src="/images/vosa_1.png" 
            alt="Vosa Sound System Logo" 
            class="w-64 h-64 mx-auto object-contain filter"
            onerror="this.style.display='none'; this.nextElementSibling.style.display='flex'"
          >
          <!-- Fallback if logo not found -->
          <div class="w-64 h-64 mx-auto bg-white/20 rounded-full flex items-center justify-center text-6xl" style="display:none;">
            👑
          </div>
        </div>
        
        <!-- Main Heading -->
        <h1 class="text-black text-5xl md:text-7xl font-bold mb-6;">
        VOSA SOUND SYSTEM
        </h1>

        <p class="text-black mt-10 mb-12">Stay tuned.<br/>The site is comming.<br/>Soon or later.</p>
      

      </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black text-white py-12">
      <div class="container mx-auto px-4 text-center">
        <p class="text-lg mb-2">&copy; {{ new Date().getFullYear() }} VOSA sound system</p>
        <p class="text-gray-400">Home of TEKK • All rights reserved</p>
      </div>
    </footer>
  </div>
</template>

<script setup>
// SEO Meta tags for VOSA Sound System
useHead({
  title: 'VOSA Sound System - Home of TEKK',
  meta: [
    { name: 'description', content: 'VOSA Sound System - Professional sound equipment and TEKK music production. Coming soon.' },
    { name: 'keywords', content: 'VOSA, sound system, TEKK, electronic music, sound equipment, audio production, music, beats, DJ' },
    { name: 'author', content: 'VOSA Sound System' },
    { property: 'og:title', content: 'VOSA Sound System - Home of TEKK' },
    { property: 'og:description', content: 'VOSA Sound System - Professional sound equipment and TEKK music production. Stay tuned for the launch.' },
    { property: 'og:type', content: 'website' },
    { property: 'og:image', content: '/vosa_1.png' },
    { name: 'twitter:card', content: 'summary_large_image' },
    { name: 'twitter:title', content: 'VOSA Sound System - Home of TEKK' },
    { name: 'twitter:description', content: 'VOSA Sound System - Professional sound equipment and TEKK music production. Coming soon.' }
  ],
  script: [
    {
      type: 'application/ld+json',
      innerHTML: JSON.stringify({
        '@context': 'https://schema.org',
        '@type': 'Organization',
        name: 'VOSA Sound System',
        description: 'Professional sound equipment and TEKK music production',
        url: 'https://vosa-sound.com',
        logo: '/vosa_1.png',
        sameAs: [],
        potentialAction: {
          '@type': 'ListenAction',
          target: {
            '@type': 'EntryPoint',
            name: 'VOSA Sound System',
            description: 'Home of TEKK music'
          }
        },
        additionalType: 'MusicGroup'
      })
    }
  ]
})
</script>