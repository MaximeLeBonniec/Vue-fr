<template>
  <div class="contact">
	<h2>Contactez nous</h2>
	<p>Adresse : {{ address }}</p>
	<p>Téléphone : {{ phone }}</p>
	<p>Email : {{ email }}</p>
	<p>Horaires :</p>
	<ul>
		<li>L-V: 06:00 à 16:00</li>
		<li>Samedi: 07:00 à 14:00</li>
		<li>Dimanche: 07:00 à 12:00</li>
	</ul>
	<footer class="footer">
		<p>{{ copyright }}</p>
	</footer>
  </div>
</template>

<script>


export default {
  name: 'ContactView',
	computed: {
		copyright() {
			const currentYear = new Date().getFullYear()

			return `Copyright ${this.restaurantName} ${currentYear}`
		}
	}
}
</script>

<style lang="scss">
#app {
	font-family: "Avenir", Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}
</style>