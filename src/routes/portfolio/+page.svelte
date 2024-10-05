<script lang="ts">
	

	const colImages1 = [
		{
			alt: "Bookhub Inventory Framework",
			src: "Images/bookhubinventory1.png",
			description: "Bookhub Inventory Framework - Version 1",
		},
		{
			alt: "Bookhub Inventory Framework",
			src: "Images/bookhubinventory2.png",
			description: "Bookhub Inventory Framework - Version 2",
		},
		{
			alt: "Bookhub Inventory Framework",
			src: "Images/bookhubinventory3.png",
			description: "Bookhub Inventory Framework - Version 3",
		},
		{
			alt: "Lab Activity",
			src: "Images/labactivity.png",
			description: "Lab Activity - Networking Experiment",
		},
	];

	const colImages2 = [
		{
			alt: "Bookhub Inventory Framework",
			src: "Images/bookhubinventory4.png",
			description: "Bookhub Inventory Framework - Version 4",
		},
		{
			alt: "Bookhub Inventory",
			src: "Images/bookhubinventory5.png",
			description: "Bookhub Inventory Interface Design",
		},
		{
			alt: "Bookhub Inventory Management System",
			src: "Images/BookInventoryManagementSystem.png",
			description: "Bookhub Inventory Management System Overview",
		},
		{
			alt: "Career Path in IT",
			src: "Images/CareerPathsinIT.png",
			description: "Career Path in Information Technology Presentation",
		},
		{
			alt: "Valdez Catering",
			src: "Images/valdezcatering1.png",
			description: "Valdez Catering Website - Home Page",
		},
		{
			alt: "Valdez Catering",
			src: "Images/valdezcatering2.png",
			description: "Valdez Catering Website - Menu Page",
		},
	];

	const colImages3 = [
		{
			alt: "CEPA",
			src: "Images/cepa.png",
			description: "CEPA - Community Engagement Platform",
		},
		{
			alt: "CEPA Feedback",
			src: "Images/cepafeedback1.png",
			description: "CEPA Feedback System Interface",
		},
		{
			alt: "Connect 4",
			src: "Images/Connect4.png",
			description: "Connect 4 Game Implementation",
		},
		{
			alt: "Ecommerce Cart",
			src: "Images/ecommercecart.png",
			description: "Ecommerce Cart Page",
		},
		{
			alt: "Ecommerce Home",
			src: "Images/ecommercehome.png",
			description: "Ecommerce Home Page",
		},
		{
			alt: "Ecommerce Warframe",
			src: "Images/ecommwarframe1.png",
			description: "Ecommerce Warframe Storefront",
		},
		{
			alt: "Messaging App",
			src: "Images/messagingapp1.png",
			description: "Messaging App Interface Design",
		},
	];
</script>

<h1 class="text-4xl">Portfolio</h1>
<p>Here are my projects and activities that I can find from the past 3 years.</p>

<div class="w-full max-w-4xl">
    <div class="grid gap-4 grid-cols-1 md:grid-cols-2 md:px-8 lg:p-0 lg:grid-cols-4">
        <div class="flex flex-col gap-4">
            {#each colImages1 as colImage}
            <div class="w-full h-fit overflow-hidden rounded-lg">
                <img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
                <p class="text-center text-white mt-2">{colImage.description}</p>
            </div>
            {/each}
        </div>
        <div class="flex flex-col gap-4">
            {#each colImages2 as colImage}
            <div class="w-full h-fit overflow-hidden rounded-lg">
                <img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
                <p class="text-center text-white mt-2">{colImage.description}</p>
            </div>
            {/each}
        </div>
        <div class="md:col-span-2 flex flex-col gap-4">
            {#each colImages3 as colImage}
            <div class="w-full h-fit overflow-hidden rounded-lg">
                <img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
                <p class="text-center text-white mt-2">{colImage.description}</p>
            </div>
            {/each}
        </div>
    </div>
</div>
