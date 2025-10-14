<template>
  <div class="min-h-screen bg-background">
    <!-- Header -->
    <Header />
    
    <!-- Main Content -->
    <main>
      <HeroSection />
      <ServicesSection />
      <MissionSection />
      <TestimonialsSection />
      <BlogSection />
      <ContactSection />
    </main>
    
    <!-- Footer -->
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import HeroSection from './components/HeroSection.vue'
import ServicesSection from './components/ServicesSection.vue'
import MissionSection from './components/MissionSection.vue'
import TestimonialsSection from './components/TestimonialsSection.vue'
import BlogSection from './components/BlogSection.vue'
import ContactSection from './components/ContactSection.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    HeroSection,
    ServicesSection,
    MissionSection,
    TestimonialsSection,
    BlogSection,
    ContactSection,
    Footer
  }
}
</script>
