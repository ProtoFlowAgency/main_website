<template>
  <section id="home" class="banner-area banner-style-one banner-bg-1 hero__area-3 banner__jump rt-hBanner relative overflow-hidden">
    <!-- Shape Image -->
    <div class="shape-image absolute top-0 right-0 w-64 h-64 opacity-10">
      <div class="w-full h-full bg-primary rounded-full"></div>
    </div>
    
    <!-- Top Center Circle -->
    <div class="top-center-image rts-scroll-down-circle-wrapper-3 rt-circle-path absolute top-1/2 right-8 transform -translate-y-1/2">
      <a href="#services" class="speen-shape scroll-down-circle-3 block w-32 h-32 relative group">
        <svg class="uni-circle-text-path uk-text-secondary uni-animation-spin w-full h-full" viewBox="0 0 100 100" width="180" height="180">
          <defs>
            <path id="circle" d="M 50, 50 m -37, 0 a 37,37 0 1,1 74,0 a 37,37 0 1,1 -74,0"></path>
          </defs>
          <text font-size="11.75" fill="currentColor" class="text-primary">
            <textPath xlink:href="#circle">Our Services •••••• Reach your Peak ••••••</textPath>
          </text>
        </svg>
        <svg aria-hidden="true" class="e-font-icon-svg e-fas-hiking absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-8 h-8 text-primary" viewBox="0 0 384 512" xmlns="http://www.w3.org/2000/svg">
          <path d="M80.95 472.23c-4.28 17.16 6.14 34.53 23.28 38.81 2.61.66 5.22.95 7.8.95 14.33 0 27.37-9.7 31.02-24.23l25.24-100.97-52.78-52.78-34.56 138.22zm14.89-196.12L137 117c2.19-8.42-3.14-16.95-11.92-19.06-43.88-10.52-88.35 15.07-99.32 57.17L.49 253.24c-2.19 8.42 3.14 16.95 11.92 19.06l63.56 15.25c8.79 2.1 17.68-3.02 19.87-11.44zM368 160h-16c-8.84 0-16 7.16-16 16v16h-34.75l-46.78-46.78C243.38 134.11 228.61 128 212.91 128c-27.02 0-50.47 18.3-57.03 44.52l-26.92 107.72a32.012 32.012 0 0 0 8.42 30.39L224 397.25V480c0 17.67 14.33 32 32 32s32-14.33 32-32v-82.75c0-17.09-6.66-33.16-18.75-45.25l-46.82-46.82c.15-.5.49-.89.62-1.41l19.89-79.57 22.43 22.43c6 6 14.14 9.38 22.62 9.38h48v240c0 8.84 7.16 16 16 16h16c8.84 0 16-7.16 16-16V176c.01-8.84-7.15-16-15.99-16zM240 96c26.51 0 48-21.49 48-48S266.51 0 240 0s-48 21.49-48 48 21.49 48 48 48z" fill="currentColor"></path>
        </svg>
      </a>
    </div>
    
    <div class="container mx-auto px-4 py-20">
      <div class="row">
        <div class="col-lg-9 max-w-4xl">
          <div class="banner-one-wrapper rt-hBanner-title">
            <h1 class="title rts_hero__title text-5xl md:text-7xl font-bold text-primary mb-8 leading-tight">
              <span class="inline-block">▴</span> 
              <span class="inline-block">M</span>
              <span class="inline-block">a</span>
              <span class="inline-block">r</span>
              <span class="inline-block">k</span>
              <span class="inline-block">e</span>
              <span class="inline-block">t</span>
              <span class="inline-block">i</span>
              <span class="inline-block">n</span>
              <span class="inline-block">g</span> 
              <span class="inline-block">▴</span> 
              <span class="inline-block">B</span>
              <span class="inline-block">u</span>
              <span class="inline-block">s</span>
              <span class="inline-block">i</span>
              <span class="inline-block">n</span>
              <span class="inline-block">e</span>
              <span class="inline-block">s</span>
              <span class="inline-block">s</span> 
              <br>
              <span class="inline-block">▴</span> 
              <span class="inline-block">E</span>
              <span class="inline-block">v</span>
              <span class="inline-block">e</span>
              <span class="inline-block">n</span>
              <span class="inline-block">t</span>
              <span class="inline-block">s</span>
            </h1>
            
            <div class="para-wraph mb-8">
              <p class="text-xl md:text-2xl text-accent leading-relaxed">
                Summit can get you there.<br>
                We are a Marketing and Business consulting service<br>
                with the expertise and talent to get you where you want to go.
              </p>
            </div>
            
            <div class="bannerJump_animation banner-jump-button rts-scroll-down-circle-wrapper-4">
              <div class="jump__anim rts_round_btn_wrap scroll-down-circle-4">
                <div class="rts-mouse-move-button">
                  <div class="btn_wrapper">
                    <a href="#services" class="rts-btn-mouse-move btn-hover btn-item inline-flex items-center justify-center px-8 py-4 bg-primary text-background rounded-lg hover:bg-accent transition-colors duration-300 group">
                      <span class="text-center">
                        Our <br> Services
                      </span>
                      <i aria-hidden="true" class="rt rt-arrow-up-right ml-2 group-hover:translate-x-1 group-hover:-translate-y-1 transition-transform duration-300">
                        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 17L17 7M17 7H7M17 7V17"></path>
                        </svg>
                      </i>
                    </a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HeroSection'
}
</script>
