<template>
    <div v-if="showOverlay" class="search-overlay">
      <div class="search-box">
        <input type="text" placeholder="Search..." class="search-input" />
        <button class="btn search-btn">SEARCH</button>
        <button @click="hideOverlay" class="close-btn">X</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        showOverlay: false
      };
    },
    methods: {
      hideOverlay() {
        this.showOverlay = false;
      }
    },
    mounted() {
      // Show the overlay when the search icon is clicked
      // You can adapt this to your own logic or event emitter
      document.querySelector('.search-icon').addEventListener('click', () => {
        this.showOverlay = true;
      });
    }
  }
  </script>
  
  <style scoped>
  .search-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .search-box {
    padding: 20px;
    background-color: #ffffff;
    border-radius: 10px;
    width: 80%;
    max-width: 500px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .search-input {
    flex: 1;
    margin-right: 10px;
    padding: 5px 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
  }
  
  .search-btn {
    background-color: #ffc107;
    border: none;
    padding: 5px 15px;
    border-radius: 5px;
    cursor: pointer;
  }
  
  .close-btn {
    background: none;
    border: none;
    font-size: 20px;
    cursor: pointer;
    margin-left: 10px;
  }
  </style>
  