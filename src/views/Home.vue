<template>
	<div class="home">
		<HeroImage v-bind:heroImage="'../assets/nails-snow.jpg'"/>
		<Nav />
		<Description />
		<CardImages />
		<Programare />
		<Testimonials />
		<Footer />		
	</div>
</template>

<script>
// @ is an alias to /src
import HeroImage from '../components/HeroImage';
import Nav from '../components/Nav';
import CardImages from '../components/CardImages';
import Description from '../components/Description';
import Programare from '../components/Programare';
import Testimonials from '../components/Testimonials';
import Footer from '../components/Footer';

export default {
  name: 'Home',
  components: {
	HeroImage,
	Nav,
	CardImages,
	Description,
	Programare,
	Testimonials,
	Footer,
  }
}
</script>

<style>
	.home {
		height: 100%;
	}
</style>