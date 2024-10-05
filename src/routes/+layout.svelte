<script>
	import "../app.css";
</script>

<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com">
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
	<link href="https://fonts.googleapis.com/css2?family=Playwrite+DE+Grund:wght@100..400&display=swap" rel="stylesheet">
</svelte:head>

<div class="min-h-screen min-w-screen flex flex-col bg-black">
	<!-- Header/Navbar -->
	<div class="flex gap-10 items-center justify-end bg-orange-400 text-white px-10 py-6 shadow-lg">
		<a href="/" class="mr-auto font-bold text-2xl text-white hover:text-yellow-400 transition-colors">
			John Christian V. Valdez
		</a>
		<a href="/about" class="text-lg hover:text-yellow-300 transition-colors">About</a>
		<a href="/portfolio" class="text-lg hover:text-yellow-300 transition-colors">Portfolio</a>
		<a href="/contact" class="text-lg hover:text-yellow-300 transition-colors">Contact</a>
	</div>

	<!-- Main Content Area -->
	<main class="flex-1 p-8 bg-black flex flex-col gap-6 justify-center items-center text-white">
		<slot></slot>
	</main>
</div>
