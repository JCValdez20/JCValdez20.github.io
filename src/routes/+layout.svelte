<script>
	import "../app.css";
</script>

<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
	<link href="https://fonts.googleapis.com/css2?family=Figtree:ital,wght@0,300..900;1,300..900&display=swap" rel="stylesheet" />
</svelte:head>

<div class="min-h-screen min-w-screen flex flex-col bg-gray-900">
	<!-- Header/Navbar -->
	<div class="flex gap-10 items-center justify-end bg-gray-800 text-gray-100 px-10 py-6 shadow-lg">
		<a href="/" class="mr-auto font-bold text-2xl text-primary-300 hover:text-white transition-colors">
			John Christian V. Valdez
		</a>
		<a href="/about" class="text-lg hover:text-primary-300 transition-colors">About</a>
		<a href="/portfolio" class="text-lg hover:text-primary-300 transition-colors">Portfolio</a>
		<a href="/contact" class="text-lg hover:text-primary-300 transition-colors">Contact</a>
	</div>

	<!-- Main Content Area -->
	<main class="flex-1 p-8 bg-gray-900 flex flex-col gap-6 justify-center items-center text-white">
		<slot></slot>
	</main>
</div>

