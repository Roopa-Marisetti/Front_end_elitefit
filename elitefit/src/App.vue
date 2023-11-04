<!-- <template>
  <HeaderSection/>
  <ContentSection/>
  <AboutSection/>
  <TestimonialsSection/>
  <FooterSection/>
</template>

<script>
import HeaderSection from './components/HeaderSection.vue'
import ContentSection from './components/ContentSection.vue'
import AboutSection from './components/AboutSection.vue'
import TestimonialsSection from './components/TestimonialsSection.vue'
import FooterSection from './components/FooterSection.vue'

export default {
  name: 'App',
  components: {
    HeaderSection,
    ContentSection,
    AboutSection,
    TestimonialsSection,
    FooterSection
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
} 
 </style> -->
<template>
  <div class="container mt-5">
    <h2 class="mb-4">Testimonials</h2>
    <div v-if="loading">Loading...</div>
    <div v-else class="row">
      <div class="col-md-3 mb-4" v-for="testimonial in testimonials" :key="testimonial.name">
        <div class="card">
          <img :src="testimonial.image" alt="testimonial image" class="card-img-top">
          <div class="card-body">
            <h5 class="card-title">{{ testimonial.name }}</h5>
            <p class="card-text">{{ testimonial.message }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      testimonials: [],
      loading: true
    };
  },
  mounted() {
    fetch('https://elitefit4you.com/test-api/testimonials.json')
      .then(response => response.json())
      .then(data => {
        this.testimonials = data.testimonials;
        this.loading = false;
      });
  }
}
</script>

<style scoped>
/* Add any additional styling here */
</style>
