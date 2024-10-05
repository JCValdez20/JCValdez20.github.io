<script lang="ts">
	const socials = [
		{ site: "https://jcvaldez20.github.io/", text: "GitHub", icon: "github" },
		{ site: "https://www.facebook.com/profile.php?id=61560380601157", text: "Facebook", icon: "facebook" },
		{ site: "christianvaldez698@gmail.com", text: "Email", icon: "mail" },
	];

	// Function to return SVG icons based on the provided icon name
	function getIcon(icon: string) {
		const icons: Record<string, string> = {
			github: `<svg xmlns="http://www.w3.org/2000/svg" class="w-16 h-16" viewBox="0 0 24 24" fill="white"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.387.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.726-4.042-1.61-4.042-1.61-.546-1.387-1.332-1.757-1.332-1.757-1.09-.745.084-.729.084-.729 1.205.084 1.84 1.236 1.84 1.236 1.07 1.835 2.809 1.304 3.495.998.108-.775.418-1.305.76-1.605-2.665-.304-5.466-1.332-5.466-5.93 0-1.31.469-2.381 1.236-3.221-.124-.303-.536-1.523.117-3.176 0 0 1.008-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.29-1.552 3.298-1.23 3.298-1.23.653 1.653.242 2.873.118 3.176.77.84 1.236 1.911 1.236 3.221 0 4.61-2.803 5.624-5.475 5.922.43.372.815 1.102.815 2.222 0 1.606-.015 2.896-.015 3.286 0 .322.218.694.825.576C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg>`,
			facebook: `<svg xmlns="http://www.w3.org/2000/svg" class="w-16 h-16" viewBox="0 0 24 24" fill="white"><path d="M22.675 0h-21.35c-.734 0-1.325.591-1.325 1.325v21.351c0 .733.591 1.324 1.325 1.324h11.494v-9.294h-3.123v-3.622h3.123v-2.672c0-3.1 1.894-4.788 4.659-4.788 1.325 0 2.463.099 2.794.143v3.24h-1.916c-1.504 0-1.794.715-1.794 1.762v2.315h3.587l-.467 3.622h-3.12v9.294h6.116c.734 0 1.325-.591 1.325-1.324v-21.35c0-.734-.591-1.325-1.325-1.325z"/></svg>`,
			mail: `<svg xmlns="http://www.w3.org/2000/svg" class="w-16 h-16" viewBox="0 0 24 24" fill="white"><path d="M12 12.713l-11.986-6.713v-2.156l11.986 6.713 11.986-6.713v2.156l-11.986 6.713zm11.986-7.713h-23.972c-1.105 0-2.014.896-2.014 2v14c0 1.105.896 2 2.014 2h23.972c1.105 0 2.014-.896 2.014-2v-14c0-1.104-.896-2-2.014-2z"/></svg>`
		};
		return icons[icon] || '';
	}
</script>

<section class="mt-0 space-y-4">
	<h1 class="text-center font-bold text-4xl">Contact Me</h1>
	<ul class="flex justify-center gap-10 mt-0">
		{#each socials as social}
			<li>
				<a href={social.site} class="flex items-center p-4 bg-gray-800 hover:bg-gray-700 text-white rounded-full" target="_blank" rel="noopener noreferrer" aria-label={social.text}>
					{@html getIcon(social.icon)}
				</a>
			</li>
		{/each}
	</ul>
</section>
