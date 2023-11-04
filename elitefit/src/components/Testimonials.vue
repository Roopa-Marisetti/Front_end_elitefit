<template>
    <div class="container">
      <div class="my-4">
        <h1>TESTIMONIALS</h1>
      </div>
      <div class="row" >
        <div class="testimonial testimonial-1 col-md-3 col-sm-12">
        </div>
        <div class="testimonial testimonial-2 col-md-3 col-sm-12">
        </div>
        <div class="testimonial testimonial-3 col-md-3 col-sm-12">
        </div>
        <div class="testimonial testimonial-4 col-md-3 col-sm-12">
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'TestimonialsSection',
  }
  </script>

<style scoped>
.testimonial{
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
  height: 35vh;
}
.testimonial-1{
  background-image: url("elitefit\src\assets\alex.png");
}
.testimonial-1:hover{
  background-image: url("elitefit\src\assets\Alex background.png");
}

.testimonial-2{
  background-image: url("elitefit\src\assets\emily.png");
}
.testimonial-2:hover{
  background-image: url("elitefit\src\assets\Emily_backgr.png");
}

.testimonial-3{
  background-image: url("elitefit\src\assets\David.png");
}
.testimonial-3:hover{
  background-image: url("elitefit\src\assets\Davig_backgr.png");
}

.testimonial-4{
  background-image: url("elitefit\src\assets\Lisa.png.png");
}
.testimonial-4:hover{
  background-image: url("elitefit\src\assets\Lisa_backgr.png");
}
</style>