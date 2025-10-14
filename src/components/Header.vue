<template>
  <header class="bg-background border-b border-accent/20 sticky top-0 z-50">
    <div class="container mx-auto px-4">
      <nav class="flex items-center justify-between py-4">
        <!-- Logo -->
        <div class="flex items-center space-x-2">
          <div class="w-8 h-8 bg-primary rounded-full flex items-center justify-center">
            <span class="text-background font-bold text-lg">S</span>
          </div>
          <span class="text-xl font-bold text-primary">Summit</span>
        </div>

        <!-- Desktop Navigation -->
        <div class="hidden md:flex items-center space-x-8">
          <a href="#home" class="text-primary hover:text-accent transition-colors">Home</a>
          <a href="#about" class="text-primary hover:text-accent transition-colors">About Us</a>
          <div class="relative group">
            <button class="text-primary hover:text-accent transition-colors flex items-center space-x-1">
              <span>Services</span>
              <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path>
              </svg>
            </button>
            <div class="absolute top-full left-0 mt-2 w-48 bg-background border border-accent/20 rounded-lg shadow-lg opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-300">
              <a href="#marketing" class="block px-4 py-2 text-primary hover:bg-accent/10">Marketing</a>
              <a href="#business" class="block px-4 py-2 text-primary hover:bg-accent/10">Business</a>
              <a href="#events" class="block px-4 py-2 text-primary hover:bg-accent/10">Events</a>
            </div>
          </div>
          <a href="#learn" class="text-primary hover:text-accent transition-colors">Learn</a>
          <a href="#contact" class="text-primary hover:text-accent transition-colors">Contact Us</a>
        </div>

        <!-- Mobile Menu Button -->
        <button @click="toggleMobileMenu" class="md:hidden p-2">
          <svg class="w-6 h-6 text-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path v-if="!mobileMenuOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
            <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
          </svg>
        </button>
      </nav>

      <!-- Mobile Navigation -->
      <div v-if="mobileMenuOpen" class="md:hidden border-t border-accent/20 py-4">
        <div class="flex flex-col space-y-4">
          <a href="#home" class="text-primary hover:text-accent transition-colors">Home</a>
          <a href="#about" class="text-primary hover:text-accent transition-colors">About Us</a>
          <div class="space-y-2">
            <span class="text-primary font-medium">Services</span>
            <div class="ml-4 space-y-2">
              <a href="#marketing" class="block text-accent hover:text-primary transition-colors">Marketing</a>
              <a href="#business" class="block text-accent hover:text-primary transition-colors">Business</a>
              <a href="#events" class="block text-accent hover:text-primary transition-colors">Events</a>
            </div>
          </div>
          <a href="#learn" class="text-primary hover:text-accent transition-colors">Learn</a>
          <a href="#contact" class="text-primary hover:text-accent transition-colors">Contact Us</a>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import { ref } from 'vue'

export default {
  name: 'Header',
  setup() {
    const mobileMenuOpen = ref(false)

    const toggleMobileMenu = () => {
      mobileMenuOpen.value = !mobileMenuOpen.value
    }

    return {
      mobileMenuOpen,
      toggleMobileMenu
    }
  }
}
</script>
