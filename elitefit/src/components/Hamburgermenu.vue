<template>
    <div>
      <!-- Hamburger Menu Button -->
      <b-button v-b-toggle.overlay-menu class="hamburger-button">☰</b-button>
  
      <!-- Overlay Menu -->
      <b-sidebar id="overlay-menu" title="Menu" no-header bg-variant="light" text-variant="dark" shadow>
        <div class="custom-menu">
          <b-nav stacked>
            <b-nav-item href="#">NEW</b-nav-item>
            <b-nav-item href="#">BRANDS</b-nav-item>
            <b-nav-item href="#" @click="closeOverlayAndScrollToAbout">ABOUT</b-nav-item>
            <b-nav-item href="#">COLLECTIONS</b-nav-item>
            <b-nav-item href="#">ACCESSORIES</b-nav-item>
          </b-nav>
        </div>
        <b-button close class="close-button" @click="() => $bvSidebar.hide('overlay-menu')"></b-button>
      </b-sidebar>
  
      <!-- Main Content (Add your content here) -->
  
      <!-- Feedback Button -->
      <button class="feedback-btn">Feedback</button>
  
      <!-- About Section -->
      <div id="about-section">
        <!-- Your about content here -->
      </div>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      closeOverlayAndScrollToAbout() {
        this.$bvSidebar.hide('overlay-menu');
        let aboutElement = document.getElementById("about-section");
        aboutElement.scrollIntoView({ behavior: "smooth" });
      }
    }
  }
  </script>
  
  <style scoped>
  .hamburger-button {
    position: fixed;
    top: 20px;
    left: 20px;
    z-index: 9999; /* Keep it on top of other elements */
  }
  
  .feedback-btn {
    position: fixed;
    bottom: 20px;
    right: 20px;
    z-index: 9998; /* Keep it below the hamburger but above other elements */
  }
  
  .custom-menu {
    width: 254px;
    height: 300px;
    padding: 10px;
    box-sizing: border-box;
    position: relative;
  }
  
  .close-button {
    position: absolute;
    top: 10px;
    right: 10px;
  }
  </style>
  