<template>
	<div class="pad65"></div>
	<div class="contacts">
		<div class="row">
			<div class="col-12 col-sm-6 col-md-6 col-xl-6">
				<img class="w-100" alt="map" src="../assets/map.png">
      </div>
      
			<div class="contacts-text col-12 col-sm-6 col-md-6 col-xl-6 pt-3">
				<h1>контакты</h1>
				
        <div class="phone">
					<a href="tel:+79999999999">
						+7 (999) 999-99-99
					</a>
				</div>
				
        <div class="mail">
					<a href="mailto:yokicafe@gmail.ru">
						yokicafe@gmail.ru
					</a>
				</div>
				
				<div>
					<h1 class="d-none d-md-block">часы работы</h1>
					<p class="d-md-none">часы работы</p>
					<p>
						вс - чт: 12:00 - 22:00
						<br>
						пт - сб: 12:00 - 23:30
					</p>
				</div>
        
        <div>
					<h1 class="d-none d-md-block">адрес</h1>
					<p class="d-md-none">адрес</p>
					<p>
						Санкт-Петербург
						<br>
						ул. Жуковского, 28
					</p>
				</div>
      </div>
    </div>
		
	</div>
</template>

<style scope>
.pad65 {
  padding-top: 65px; 
}

.contacts-text {
	padding: 0px 32px 0px 32px;
  text-align: left;
}

a {
	font-size: 21px;
  color: #D9D9D9;
  font-family: 'Montserrat';
  font-weight: 300; 
  line-height: 1.2;
  margin-top: 10px; 
  margin-bottom: 15px;
}

h1 {
  font-size: 56px;
  color: #fFE239;
  font-family: 'Montserrat';
  font-weight: 900; 
  text-transform: lowercase;
}

p {
  font-size: 21px;
  color: #D9D9D9;
  font-family: 'Montserrat';
  font-weight: 300; 
  line-height: 1.2;
  margin-top: 10px; 
  margin-bottom: 15px;
}
</style>