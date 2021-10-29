<template>
	<div class="admin-main">
		<header-admin></header-admin>
	    <div class="container-fluid">
	      <div class="row">
	        
	        <nav-admin></nav-admin>

	        <main role="main" class="col-md-9 ml-sm-auto col-lg-10 pt-3 px-4">
	          <Nuxt />
	        </main>
	      </div>
	    </div>
	</div><!--end of admin-main-->
</template>
<script>
	import HeaderAdmin from '~/components/admin/shared/HeaderAdmin';
	import NavAdmin from '~/components/admin/shared/NavAdmin';
	export default {
		components : {
			'header-admin' : HeaderAdmin,
			'nav-admin' : NavAdmin
		},
		head(){
			return {
				link : [
					{ rel : 'stylesheet', href : '/admin/css/style.css'}
				]
			}
		}
	}
</script>