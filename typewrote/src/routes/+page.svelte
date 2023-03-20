<script>
	import { src_url_equal } from 'svelte/internal';
	import { Typewriter } from 'sveltyped';
	import Seo from './Seo.svelte';
	let words = ['hello', 'svelte community!'];
</script>

<div>
	<h1 class="no-loop">
		<Typewriter phrases={words} loop={false} />
	</h1>

	<h2>
		<Typewriter
			phrases={[
				'This is a demo of the sveltyped library. this time we have loop on and faster type speed.',
				'pretty cool right?'
			]}
			loop={true}
			typeSpeed={80}
		/>
	</h2>
	<h3>
		<Typewriter
			phrases={[
				'now we have it colored and with a different font',
				'if you want to have it loop once and for the text to stay u may have to do an if statement if u have multiple items in the array'
			]}
			loop={true}
			typeSpeed={60}
		/>
	</h3>
</div>

<div class="img-outer">
	<div class="img-div">
		<h4>created by:</h4>
		<img
			src="https://media.discordapp.net/attachments/560606477241417729/1087380635963883604/me.png"
			alt="3d render of shaked lanciano"
		/>

		<h2>Shaked Lanciano</h2>
		<p>junior front end developer.</p>
		<p>Email: shakedlanciano@gmail.com</p>
	</div>
</div>

<Seo />

<style>
	div {
		margin: 0 auto;
		text-align: center;
		max-width: 800px;
		padding: 10rem 5rem;
	}

	h3 {
		font-family: 'courier new', cursive;
		font-size: 1.5rem;
		color: rgb(138, 138, 138);
	}

	img {
		width: 5rem;
	}

	.img-div {
		padding: 1rem 2rem;
		margin-top: 1rem;
		border: 1px solid grey;
		border-radius: 10px;
	}
</style>
