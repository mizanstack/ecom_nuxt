<template>
	<div class="index-admin">
        <h2>Create Product</h2>
        <div class="index-content">
        	<form @submit.prevent="saveData()">
			  <div class="form-group">
			    <label for="product-name">Name</label>
			    <input type="text" class="form-control" id="product-name" placeholder="Enter Your product name">
			  </div>

			  <div class="form-group">
			    <label for="product-price">Price</label>
			    <input type="number" class="form-control" id="product-price" placeholder="10">
			  </div>

			  <div class="form-group">
			    <label for="product-qty">Qty</label>
			    <input type="number" class="form-control" id="product-qty" placeholder="Stock Qty">
			  </div>

			  <div class="form-group">
			    <label for="product-image">Image</label>
			    <input type="file" class="form-control-file" id="product-image">
			  </div>

			  <div class="form-group">
			  	<button type="submit" class="btn btn-primary">Submit</button>
			  </div>
			</form>
        </div><!--end of index-content-->
	</div><!--end of index-admin-->
</template>
<script>
	export default {
		layout : 'admin',
		data(){
			return {
				formData : {
					name : '',
					price : '',
					qty : '',
					image : ''
				},
				formErrors : {},
			}
		},
		methods : {
			saveData(){
				this.$axios.post('products', this.formData).then((response) => {
					console.log(response);
				});
			}
		}
	}
</script>