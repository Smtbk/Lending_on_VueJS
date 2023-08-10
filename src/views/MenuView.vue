<template>
	<div class="pad65"></div>
  <div class="menu">
		<div class="menu-head">
			<h1>меню</h1>
		</div>
		
		<div id="carousel-menu" class="carousel slide carousel-slide w-100">
    
      <div class="carousel-indicators">
        <button type="button" 
          data-bs-target="#carousel-menu" 
          data-bs-slide-to="0" 
          class="active">
        </button>
        <button type="button" 
          data-bs-target="#carousel-menu" 
          data-bs-slide-to="1">
        </button>
        <button type="button" 
          data-bs-target="#carousel-menu" 
          data-bs-slide-to="2">
        </button>
				<button type="button" 
          data-bs-target="#carousel-menu" 
          data-bs-slide-to="3">
        </button>
      </div>
      
			<div class="row">
				<div class="carousel-inner">
					<div class="col-md-6 offset-md-3">
						<div class="carousel-item active">
							<img src="../assets/menu/1.png" class="d-block w-100">
						</div>
					</div>
					<div class="col-md-6 offset-md-3">
						<div class="carousel-item">
							<img src="../assets/menu/2.png" class="d-block w-100">
						</div>
					</div>
					<div class="col-md-6 offset-md-3">
						<div class="carousel-item">
							<img src="../assets/menu/b1.png" class="d-block w-100">
						</div>
					</div>
					<div class="col-md-6 offset-md-3">
						<div class="carousel-item">
							<img src="../assets/menu/b2.png" class="d-block w-100">
						</div>
					</div>	
				</div>
			</div>
      
      <button class="carousel-control-prev prev" type="button" data-bs-target="#carousel-menu" data-bs-slide="prev">
        <span class="carousel-control-prev-icon"></span>
      </button>
      
      <button class="carousel-control-next next" type="button" data-bs-target="#carousel-menu" data-bs-slide="next">
        <span class="carousel-control-next-icon"></span>
      </button>
    </div>
  </div>
</template>

<style scope>
.pad65 {
  padding-top: 65px; 
}

.menu-head {
	text-align: center;
}

h1 {
  font-size: 56px;
  color: #fFE239;
  font-family: 'Montserrat';
  font-weight: 900; 
  text-transform: lowercase;
}

.prev:hover {
	background: linear-gradient(to right, #101010, transparent);
}

.next:hover {
	background: linear-gradient(to left, #101010, transparent);
}
</style>