<template>
  <section id="testimonials" class="py-20 bg-accent/5">
    <div class="container mx-auto px-4">
      <!-- Section Header -->
      <div class="text-center mb-16">
        <h2 class="text-4xl md:text-5xl font-bold text-primary mb-6">
          Teamwork makes<br>
          the dream work
        </h2>
        <p class="text-xl text-accent">
          Hear what our clients have to say
        </p>
      </div>

      <!-- Testimonials Horizontal Scroll -->
      <div class="flex gap-8 overflow-x-auto pb-4 scrollbar-hide">
        <div v-for="testimonial in testimonials" :key="testimonial.id" 
             class="bg-background border border-accent/20 rounded-lg p-6 hover:shadow-lg transition-shadow flex-shrink-0 w-80">
          <div class="flex items-center mb-4">
            <div class="w-12 h-12 bg-primary rounded-full flex items-center justify-center mr-4">
              <span class="text-background font-bold">{{ testimonial.name.charAt(0) }}</span>
            </div>
            <div>
              <h4 class="font-semibold text-primary">{{ testimonial.name }}</h4>
              <p class="text-sm text-accent">{{ testimonial.company }}</p>
            </div>
          </div>
          <p class="text-accent mb-4">{{ testimonial.text }}</p>
          <a href="#" class="text-primary hover:text-accent transition-colors text-sm font-semibold">
            Read more
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'TestimonialsSection',
  setup() {
    const testimonials = [
      {
        id: 1,
        name: 'Muhsin Ahmed',
        company: 'Al-Haramain Travels',
        text: 'We had the privilege of working with Summit for marketing consultancy at Al-Haramain Travels, and his expertise has been nothing short of transformative for our business. Summit provided us clear, strategic, and highly effective marketing guidance...'
      },
      {
        id: 2,
        name: 'Adil Ali',
        company: 'President, Madrasatu At-Tanzeel',
        text: 'Summit greatly enhanced our marketing and event management at Madrasatu At-Tanzeel. Their strategic approach strengthened our brand, engagement, and online presence. Their expertise in digital marketing and event execution ensured smooth, impactful outcomes.'
      },
      {
        id: 3,
        name: 'Olive Tree Events',
        company: 'www.olivetreeevents.au',
        text: 'My experience with Summit for business support has been fantastic. Their guidance and expertise made a real difference, combining meaningful perspective with practical, hands-on help. Summit took the time to really understand my vision...'
      },
      {
        id: 4,
        name: 'Joumana',
        company: 'Dusty Pink',
        text: 'I\'ve had the pleasure of attending several events where Summit has showcased their exceptional organizational skills, professionalism, and attention to detail. Your events are always well-structured, engaging, and successful.'
      },
      {
        id: 5,
        name: 'Amir Reyad',
        company: 'CEO, Antenna Genie',
        text: 'I\'ve had the pleasure of attending several events where Summit has showcased their exceptional organizational skills, professionalism, and attention to detail. Your events are always well-structured, engaging, and successful.'
      },
      {
        id: 6,
        name: 'Ahmed Elkheir',
        company: 'CEO, Plumbfast',
        text: 'I have attended several events organized by the Summit team, every time I am impressed. Their events are smooth, seamless, and the whole night flows with high energy and high impact. On more than one occasion I have been extremely moved...'
      }
    ]

    return {
      testimonials
    }
  }
}
</script>
