<template>
	<div class="pad65"></div>
	
	<div class="reservation">
		
		<form id="form" v-on:submit.prevent="sendData()" class="pb-3">
			<div class="container">
				<div class="row">
					<div class="col-12">
						<h1 class="d-none d-md-block">забронировать столик</h1>
						<h1m class="d-md-none">забронировать столик</h1m>
					</div>
				</div>
			</div>
			
			<div class="container">
				<div class="row mb-3">
					<div class="col-12 col-sm-12 col-md-6 col-lg-6 col-xl-6">
						<label for="InputName" class="form-label">Имя</label>
						<input type="name" class="form-control" id="InputName" placeholder="Александр" required>
					</div>
				</div>
				
				<div class="row mb-3">
					<div class="col-12 col-sm-12 col-md-6 col-lg-6 col-xl-6">
						<label for="leInputDate" class="form-label">Дата</label>
						<input type="date" class="form-control" id="InputDate" v-bind:value="reseraData" v-on:input="reservDataChange" required>
					</div>
				</div>
				
				<div class="row mb-3">
					<div class="col-12 col-sm-12 col-md-6 col-lg-6 col-xl-6">
						<label for="leInputNum" class="form-label">Количество гостей</label>
						<input type="number" class="form-control" id="InputNum" min="1" max="7" placeholder="Количество от 1 до 7" required>
					</div>
				</div>
				
				<div class="row mb-3">
					<div class="col-12 col-sm-12 col-md-6 col-lg-6 col-xl-6">
						<label for="leInputPhone" class="form-label">Номер телефона</label>
						<input type="tel" 
							class="form-control" 
							id="InputPhone" 
							placeholder="+7 (999) 999-99-99" 
							required>
						<div id="phoneHelp" class="form-text">Мы не станем звонить вам в рекламных целях.</div>
					</div>
				</div>
				
				<button type="submit" class="btn">Забронировать столик</button>
				
			</div>
		</form>
	</div>
	
	<ModalWin show="isModalVisible" v-on:close="closeModal"/>
	
</template>

<script>
import ModalWin from '@/components/ModalWin.vue'

export default {
	data(){
		return {
			reseraData: "",
			isModalVisible: false,
		}
	},
	methods: {
		reservDataChange(event){
			this.reseraData = event.target.value
		},
		sendData(){
			alert("Ваш столик забронирован на " + this.reseraData + ".");
		},
		showModal() {
			this.isModalVisible = true;
		},
		closeModal() {
			this.isModalVisible = false;
		}
	},
	components: {
		ModalWin
	}
}
</script>

<style scope>
.pad65 {
  padding-top: 65px; 
}

.btn {
	background-color: #fFE239;
}

.btn:hover {
	color: black;
	background-color: white;
}

h1 {
  font-size: 56px;
  color: #FFE239;
  font-family: 'Montserrat';
  font-weight: 900; 
  text-transform: lowercase;
}

h1m {
  font-size: 40px;
  color: #FFE239;
  font-family: 'Montserrat';
  font-weight: 900; 
  text-transform: lowercase;
}

form {
  font-size: 21px;
  color: #D9D9D9;
  font-family: 'Montserrat';
  font-weight: 300; 
  line-height: 1.2;
  margin-top: 10px; 
  margin-bottom: 15px;
}

.form-control:focus {
	border-color: #FFE239;
	outline: 0;
	box-shadow: 0 0 0 0.25rem #FFE239;
}
</style>