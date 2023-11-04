<template>
  <div>
    <div class="mobile-header">
      Main page - mobile
      <span class="header-info">...FREE SHIPPING ON ALL ORDERS...</span>
    </div>
    <div class="main-section">
      PISTONS
      <div class="icons">
        <span class="icon">🛒</span>
        <span class="icon">🔍</span>
        <span class="icon">☰</span>
      </div>
    </div>
    <div class="content-section">
      <div class="feedback">FEEDBACK</div>
      <img src="elitefit\src\assets\Image1.png" alt="Made for you" />
      <div class="shop-btn">SHOP PENS</div>
    </div>
  </div>
  <div class="content-section">
    <img src="elitefit\src\assets\Madefor.png" alt="Made for you" />
    <div class="shop-btn">SHOP PENS</div>
  </div>

  <div class="change-makers-section">
    <img src="elitefit\src\assets\shop brand.png" alt="Made for the best change makers" />
    <div class="shop-brands-btn">SHOP BRANDS</div>
  </div>
  
  <div class="mont-blanc-section">
    <img src="elitefit\src\assets\Shop Mont blanc.png" alt="Savour the present" />
    <div class="shop-mont-blanc-btn">SHOP MONT BLANC</div>
  </div>

  <div class="quality-class-section">
    <img src="elitefit\src\assets\Quality class.png" alt="Where quality meets class" />
    <div class="shop-fall-collection-btn">SHOP THE FALL 2023 COLLECTION</div>
  </div>
  <div class="about-pistons-section">
    <img src="elitefit\src\assets\About positions.png" alt="About Pistons" />
    <div class="about-pistons-content">
      <div class="about-pistons-title">ABOUT PISTONS</div>
      <div class="about-pistons-text">
        Established in 1897, our beloved fountain pen haven, 'PISTONS,' has been a haven for pen enthusiasts for generations. 
        With a century-long dedication to fine writing instruments, we've bridged tradition and modernity, offering a curated 
        selection of vintage and contemporary fountain pens. Our little shop, nestled in the heart of town, continues to inspire 
        a love for the art of writing, connecting past and present through the timeless elegance of ink on paper.
      </div>
    </div>
  </div>
  

</template>

<script>
export default {
  name: "MainPage",
  data() {
    
  }
}

</script>
<style scoped>


.content-section {
  width: 390px;
  height: 648px;
  position: relative;
}

.feedback {
  position: absolute;
  top: 10px;
  right: 10px;
  background-color: white;
  padding: 5px 10px;
  border: 1px solid #e0e0e0;
  font-size: 12px;
}

.shop-btn {
  position: absolute;
  bottom: 50px;
  left: 50%;
  transform: translateX(-50%);
  background-color: white;
  padding: 10px 20px;
  border: 1px solid #e0e0e0;
  cursor: pointer;
  text-align: center;
  font-size: 16px;
}
.change-makers-section {
  width: 390px;
  height: 648px;
  position: relative;
}

.shop-brands-btn {
  position: absolute;
  bottom: 50px;
  left: 50%;
  transform: translateX(-50%);
  background-color: white;
  padding: 10px 20px;
  border: 1px solid #e0e0e0;
  cursor: pointer;
  text-align: center;
  font-size: 16px;
}
.mont-blanc-section {
  width: 390px;
  height: 648px;
  position: relative;
}
.shop-mont-blanc-btn {
  position: absolute;
  bottom: 50px;
  left: 50%;
  transform: translateX(-50%);
  background-color: white;
  padding: 10px 20px;
  border: 1px solid #e0e0e0;
  cursor: pointer;
  text-align: center;
  font-size: 16px;
}
.quality-class-section {
  width: 390px;
  height: 485px;
  position: relative;
}

.shop-fall-collection-btn {
  position: absolute;
  bottom: 50px;
  left: 50%;
  transform: translateX(-50%);
  background-color: white;
  padding: 10px 20px;
  border: 1px solid #e0e0e0;
  cursor: pointer;
  text-align: center;
  font-size: 16px;
}
.about-pistons-title {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
}

.about-pistons-text {
  font-size: 14px;
  line-height: 1.5;
}


</style>
