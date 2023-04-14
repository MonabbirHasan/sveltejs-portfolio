<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/ai.png';
</script>

<header class="navbar navbar-expand-lg">
	<div class="corner">
		<a href="https://kit.svelte.dev">
			<img src={logo} alt="SvelteKit" class="website-logo" />
		</a>
	</div>

	<nav class="container-fluid">
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L1,2 C1.5,3 1.5,3 2,3 L2,0 Z" />
		</svg>
		<ul>
			<li aria-current={$page.url.pathname === '/home' ? 'page' : undefined}>
				<a href="/">Home</a>
			</li>
			<li aria-current={$page.url.pathname === '/home' ? 'page' : undefined}>
				<a href="/">About</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/home') ? 'page' : undefined}>
				<a href="/">skills</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/home') ? 'page' : undefined}>
				<a href="/">portfolio</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/home') ? 'page' : undefined}>
				<a href="/">blogs</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/home') ? 'page' : undefined}>
				<a href="/">services</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/home') ? 'page' : undefined}>
				<a href="/">contact</a>
			</li>
		</ul>
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L0,3 C0.5,3 0.5,3 1,2 L2,0 Z" />
		</svg>
	</nav>

	<!-- <div class="corner">
		<a href="https://github.com/sveltejs/kit">
			<img src={github} alt="GitHub" />
		</a>
	</div> -->
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		width: 100%;
		position: absolute;
		z-index: 1000;
		padding: 0 !important;
	}
	nav.s-Cmt25qOMERl7.s-Cmt25qOMERl7{
		background-color: #fff!important;
	}
	.corner {
		width: 3em;
		height: 3em;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
	}

	.corner img {
		width: 200px;
		height: auto;
		position: relative;
		object-fit: cover;
		top: 40px;
		filter: hue-rotate(20deg);
		/* left: 31px; */
		animation: logo 1s linear infinite;
		padding-left: 83px;
	}

	nav {
		display: flex;
		justify-content: center;
		--background: rgba(255, 255, 255, 0.7);
	}

	svg {
		width: 2em;
		height: 3em;
		display: block;
	}

	path {
		fill: var(--background);
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li[aria-current='page']::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--color-theme-1);
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-theme-1);
	}
	@keyframes logo {
		0% {
			filter: hue-rotate(0deg);
		}
		90% {
			filter: hue-rotate(200deg);
		}
		100% {
			filter: hue-rotate(360deg);
		}
	}
</style>
