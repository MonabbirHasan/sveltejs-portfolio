<script>

	import Header from './Header.svelte';
	import './styles.css';
</script>

<div class="app">
	<Header />
	<main>
		<slot />
	</main>
	
	<footer>
		<!-- <nav class="d-flex">
			<ul class="menu">
				<li><a href="/home"><ion-icon name="home-outline" /></a><span>home</span></li>
				<li>
					<a href="/about"><ion-icon name="information-circle-outline" /></a><span>about</span>
				</li>
				<li><a href="/portfolio"><ion-icon name="images-outline" /></a><span>portfolio</span></li>
				<li><a href="/blog"><ion-icon name="documents-outline" /></a><span>blog</span></li>
				<li><a href="/serivec"><ion-icon name="apps-outline" /></a><span>services</span></li>
			</ul>
			<ul class="icon">
				<li><a href="/home"><ion-icon name="logo-facebook" /></a><span>facebook</span></li>
				<li><a href="/about"><ion-icon name="logo-instagram" /></a><span>instagram</span></li>
				<li><a href="/portfolio"><ion-icon name="logo-twitter" /></a><span>twitter</span></li>
				<li><a href="/blog"><ion-icon name="mail-outline" /></a><span>mail</span></li>
				<li><a href="/serivec"><ion-icon name="logo-whatsapp" /></a><span>whatsapp</span></li>
			</ul>
		</nav>
		<nav class="d-flex">
			<ul class="menu">
				<li><a href="/home"><ion-icon name="home-outline" /></a><span>home</span></li>
				<li>
					<a href="/about"><ion-icon name="information-circle-outline" /></a><span>about</span>
				</li>
				<li><a href="/portfolio"><ion-icon name="images-outline" /></a><span>portfolio</span></li>
				<li><a href="/blog"><ion-icon name="documents-outline" /></a><span>blog</span></li>
				<li><a href="/serivec"><ion-icon name="apps-outline" /></a><span>services</span></li>
			</ul>
			<ul class="icon">
				<li><a href="/home"><ion-icon name="logo-facebook" /></a><span>facebook</span></li>
				<li><a href="/about"><ion-icon name="logo-instagram" /></a><span>instagram</span></li>
				<li><a href="/portfolio"><ion-icon name="logo-twitter" /></a><span>twitter</span></li>
				<li><a href="/blog"><ion-icon name="mail-outline" /></a><span>mail</span></li>
				<li><a href="/serivec"><ion-icon name="logo-whatsapp" /></a><span>whatsapp</span></li>
			</ul>
		</nav> -->
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}
	/* main {
		display: flex;
		width: 100%;
		margin: 0 auto;
		box-sizing: border-box;
	} */

	footer {
		display: flex;
		justify-content: space-evenly;
		padding: 60px 0;
		width: 100%;
		background: #000;
	}

	/* footer a {
		font-weight: bold;
		color: white;
		font-size: 25px;
	}
	footer .icon li {
		font-size: 15px !important;
		color: white;
		list-style: none;
	}
	footer .icon li {
		line-height: 40px;
	}
	footer ul li span {
		margin-left: 10px;
		text-transform: capitalize;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	} */
	/* footer ul li {
		line-height: 20px;
	}
	.menu li {
		line-height: 40px;
	}
	.menu li a {
		font-size: 20px !important;
		font-weight: 900;
	}
	.menu li a:hover {
		color: #fc9400;
	}
	.icon li a:hover {
		color: #fc9400;
	}
	.menu li span {
		color: white;
		font-size: 15px;
	} */
</style>
