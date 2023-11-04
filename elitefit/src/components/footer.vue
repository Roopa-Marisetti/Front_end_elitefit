<template>
    <footer class="footer bg-dark text-white py-4 text-center">
      <h1 class="mb-3">PISTONS</h1>
      <h3 class="mb-3">STAY CONNECTED</h3>
      <div class="social-icons">
        <a :href="links.facebook" target="_blank" class="btn btn-dark btn-lg me-2"><i class="fab fa-facebook-f"></i></a>
        <a :href="links.youtube" target="_blank" class="btn btn-dark btn-lg me-2"><i class="fab fa-youtube"></i></a>
        <a :href="links.instagram" target="_blank" class="btn btn-dark btn-lg me-2"><i class="fab fa-instagram"></i></a>
        <a :href="links.twitter" target="_blank" class="btn btn-dark btn-lg me-2"><i class="fab fa-twitter"></i></a>
        <a :href="links.email" class="btn btn-dark btn-lg me-2"><i class="fas fa-envelope"></i></a>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    data() {
      return {
        links: {
          facebook: '../assets/facebook.png',
          youtube: '../assets/youtube.png',
          instagram: '../assets/instagram.png',
          twitter: '../assets/twitter.png',
          email: 'mailto:example@example.com'
        }
      }
    }
  }
  </script>
  