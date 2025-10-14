<template>
  <section id="learn" class="py-20 bg-background">
    <div class="container mx-auto px-4">
      <!-- Section Header -->
      <div class="text-center mb-16">
        <h2 class="text-4xl md:text-5xl font-bold text-primary mb-6">
          The Summit Digest
        </h2>
        <p class="text-xl text-accent mb-8">
          LEARN WITH US
        </p>
        <p class="text-lg text-accent max-w-2xl mx-auto">
          From the latest news, to the biggest trends in the market, here's the scoop of everything "cool"
        </p>
      </div>

      <!-- Blog Posts -->
      <div class="grid md:grid-cols-2 gap-8 mb-12">
        <article v-for="post in blogPosts" :key="post.id" 
                 class="bg-background border border-accent/20 rounded-lg overflow-hidden hover:shadow-lg transition-shadow">
          <div class="h-48 bg-accent/10 flex items-center justify-center">
            <div class="w-16 h-16 bg-primary rounded-lg flex items-center justify-center">
              <svg class="w-8 h-8 text-background" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path>
              </svg>
            </div>
          </div>
          <div class="p-6">
            <div class="flex items-center text-sm text-accent mb-3">
              <span>{{ post.date }}</span>
              <span class="mx-2">•</span>
              <span>{{ post.readTime }}</span>
            </div>
            <h3 class="text-xl font-bold text-primary mb-3">{{ post.title }}</h3>
            <p class="text-accent mb-4">{{ post.excerpt }}</p>
            <a href="#" class="text-primary hover:text-accent transition-colors font-semibold">
              Read More →
            </a>
          </div>
        </article>
      </div>

      <!-- CTA -->
      <div class="text-center">
        <a href="#" class="btn-secondary">
          VIEW BLOG
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'BlogSection',
  setup() {
    const blogPosts = [
      {
        id: 1,
        title: 'Social Media Platforms: Unique Ecosystems with Their Own Rules',
        excerpt: 'Understanding how different social media platforms operate as unique ecosystems with their own rules and best practices.',
        date: 'September 2, 2024',
        readTime: '3 minutes Read'
      },
      {
        id: 2,
        title: 'Marketing for a Good Cause: How Australian Brands Can Make a Positive Impact',
        excerpt: 'Exploring how Australian brands can leverage marketing strategies to create positive social impact and meaningful change.',
        date: 'November 26, 2023',
        readTime: '5 minutes Read'
      }
    ]

    return {
      blogPosts
    }
  }
}
</script>
