<template>
  <div>
    <div id="carousel" class="carousel slide carousel-slide w-100">
    
      <div class="carousel-indicators">
        <button type="button" 
          data-bs-target="#carousel" 
          data-bs-slide-to="0" 
          class="active">
        </button>
        <button type="button" 
          data-bs-target="#carousel" 
          data-bs-slide-to="1">
        </button>
        <button type="button" 
          data-bs-target="#carousel" 
          data-bs-slide-to="2">
        </button>
      </div>
      
      <div class="carousel-inner">
        <div class="carousel-item w-100 active">
          <img src="../assets/slider/1.png" class="d-block w-100">
        </div>
        <div class="carousel-item">
          <img src="../assets/slider/2.png" class="d-block w-100">
        </div>
        <div class="carousel-item">
          <img src="../assets/slider/3.png" class="d-block w-100">
        </div>
      </div>
      
      <button class="carousel-control-prev prev" type="button" data-bs-target="#carousel" data-bs-slide="prev">
        <span class="carousel-control-prev-icon"></span>
      </button>
      
      <button class="carousel-control-next next" type="button" data-bs-target="#carousel" data-bs-slide="next">
        <span class="carousel-control-next-icon"></span>
      </button>
    </div>
  </div>
</template>

<style scoped>
.prev:hover {
	background: linear-gradient(to right, #101010, transparent);
}

.next:hover {
	background: linear-gradient(to left, #101010, transparent);
}
</style>
