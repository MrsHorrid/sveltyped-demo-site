<script>
	import '../app.css';
</script>

<nav>
	<h1>Sveltyped.</h1>
	<ul>
		<li><a href="https://www.npmjs.com/package/sveltyped" target="_blank">NPM Website</a></li>
		<li><a href="https://github.com/MrsHorrid/Sveltyped" target="_blank">Git Repo</a></li>
	</ul>
</nav>
<main>
	<slot />
</main>

<style>
	nav {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 3rem 8rem;
		align-items: center;
	}

	ul {
		list-style: none;
		display: flex;
		gap: 2rem;
	}

	a {
		text-decoration: none;
		color: #000;
		font-size: 1rem;
	}
</style>
