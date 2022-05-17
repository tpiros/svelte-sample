<script>
	import { onMount } from 'svelte';
	onMount(() => {
		const myCloudinary = cloudinary.videoPlayer('vid-player', { cloud_name: 'tamas-demo' });
		myCloudinary.source('colombia');
	});
</script>

<svelte:head>
	<link
		href="https://unpkg.com/cloudinary-video-player@1.9.0/dist/cld-video-player.min.css"
		rel="stylesheet"
	/>
	<script
		src="https://unpkg.com/cloudinary-video-player@1.9.0/dist/cld-video-player.min.js"
		type="text/javascript"></script>
</svelte:head>
<h1>Welcome to SvelteKit</h1>
<video id="vid-player" controls muted class="cld-video-player cld-fluid" />
<a href="/about">About</a>
