<template>
	<section>
		<base-card>
			<h2>Welcome!</h2>
			<p>Uvodna stranka</p>
		</base-card>
	</section>
</template>

<script>
export default {
	name: 'IndexPage',
	mounted() {
		console.log('IndexPage mounted');
		// toto funguje ked sa preklada cez vue-cli-service
		// console.log('VUE_APP_API_KEY z ENV' + process.env.VUE_APP_API_KEY);
		console.log('VITE_API_KEY ' + import.meta.env.VITE_API_KEY);
		console.log('my-app-config ' + this.API_KEY);
	},
};


</script>