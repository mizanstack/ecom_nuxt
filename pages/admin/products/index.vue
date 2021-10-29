<template>
	<div class="index-admin">
        <h2>Products</h2>

        <NuxtLink to="/admin/products/create" class="btn btn-primary">Create</NuxtLink>
        <div class="index-content">
        	<div class="table-responsive">
			  <table class="table">
			    <thead>
			      <tr>
			        <th scope="col">#</th>
			        <th scope="col">Name</th>
			        <th scope="col">Image</th>
			        <th scope="col">Action</th>
			      </tr>
			    </thead>
			    <tbody>
			      <tr>
			        <th scope="row">1</th>
			        <td>Product 1</td>
			        <td>Product Image</td>
			        <td>
			        	<button type="button" class="btn btn-primary">Primary</button>
						<button type="button" class="btn btn-secondary">Secondary</button>
						<button type="button" class="btn btn-success">Success</button>
						<button type="button" class="btn btn-danger">Danger</button>
						<button type="button" class="btn btn-warning">Warning</button>
						<button type="button" class="btn btn-info">Info</button>
						<button type="button" class="btn btn-light">Light</button>
						<button type="button" class="btn btn-dark">Dark</button>

						<button type="button" class="btn btn-link">Link</button>
			        </td>
			      </tr>
			    </tbody>
			  </table>
			</div>
        </div><!--end of index-content-->
	</div><!--end of index-admin-->
</template>
<script>
	export default {
		layout : 'admin'
	}
</script>