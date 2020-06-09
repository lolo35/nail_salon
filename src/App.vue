<template>
	<div id="app">
		
		<router-view/>
	</div>
</template>
<script>
import 'jquery';
import 'popper.js';
import 'bootstrap';
import '../node_modules/bootstrap/dist/css/bootstrap.css';
import '../node_modules/@fortawesome/fontawesome-free/css/all.css';

	export default {
		name: 'App',

	}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
    body, html, #app{
        height: 100%;
		font-family: 'Lobster', cursive;
    }
</style>
