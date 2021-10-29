<template>
	<div class="main-front">
		<header-front></header-front>
			<Nuxt />
	    <footer-front></footer-front>
    </div>
</template>

<script>
	import HeaderFront from '~/components/front/shared/HeaderFront.vue'
	import FooterFront from '~/components/front/shared/FooterFront.vue'

	export default {
		components : {
			'header-front' : HeaderFront,
			'footer-front' : FooterFront,
		}
	}
</script>