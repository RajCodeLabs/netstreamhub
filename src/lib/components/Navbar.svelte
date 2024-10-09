<script>
	let links = [
		{
			text: "Home",
            url: "/#home",
		},
		{
			text: "Pricing",
            url: "/#pricing",
		},
		{
			text: "FAQ",
			url: "/#faq",
		},
		{
			text: "Renew",
			url: "/renew",
		},
		{
			text: "Installation Guide",
			url: "/installation",
		},
		{
			text: "Contact Us",
			url: "/#contact",
		}
		
	];
	let isMenuOpen = false;
</script>

<header class="relative flex items-center justify-between px-2 py-4">
	<!-- Logo Section -->
	<div class="flex-shrink-0">
		<a href="/" class="font-semibold">
			<span
				class="text-lg lg:text-2xl font-semibold inline-flex animate-shine bg-[linear-gradient(110deg,#939393,45%,#1e2631,55%,#939393)] bg-[length:200%_100%] text-transparent bg-clip-text"
			>
				NetStreamHub
			</span>
		</a>
	</div>

	<!-- Center Navigation (hidden on mobile) -->
	<div class="absolute left-1/2 transform -translate-x-1/2 hidden md:flex md:flex-1 md:justify-center">
		<ul class="md:flex justify-end space-y-0 md:space-x-6">
			{#each links as link}
				<li>
					<a href="{link.url}" class="block py-1 hover:text-purple-400">{link.text}</a>
				</li>
			{/each}
		</ul>
	</div>

	<!-- Free Trial Button (absolute center on small screens) -->
	<div class="absolute left-1/2 transform -translate-x-1/2 md:relative md:left-auto md:transform-none">
		<a href="https://wa.me/15551234567">
			<button
				class="group relative grid overflow-hidden rounded-xl px-4 py-2 shadow-[0_1000px_0_0_hsl(0_0%_20%)_inset] transition-colors duration-200"
			>
				<span>
					<span
						class="spark mask-gradient animate-flip before:animate-kitrotate absolute inset-0 h-[100%] w-[100%] overflow-hidden rounded-xl [mask:linear-gradient(white,_transparent_50%)] before:absolute before:aspect-square before:w-[200%] before:rotate-[-90deg] before:bg-[conic-gradient(from_0deg,transparent_0_340deg,white_360deg)] before:content-[''] before:[inset:0_auto_auto_50%] before:[translate:-50%_-15%]"
					/>
				</span>
				<span
					class="backdrop absolute inset-px rounded-[11px] bg-neutral-950 transition-colors duration-200 group-hover:bg-neutral-900"
				/>
				<span class="z-10 text-neutral-400 text-sm font-medium">Free Trial</span>
			</button>
		</a>
	</div>

	<!-- Hamburger Menu (only visible on mobile) -->
	<div class="md:hidden">
		<button class="md:hidden" on:click="{() => (isMenuOpen = !isMenuOpen)}">
			<svg
				class="w-6 h-6"
				fill="none"
				stroke="white"
				viewBox="0 0 24 24"
				xmlns="http://www.w3.org/2000/svg"
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M4 6h16M4 12h16m-7 6h7"
				></path>
			</svg>
		</button>
	</div>
</header>
 {#if isMenuOpen}
 <!-- Add opening and closing transitions -->
	<div class="md:hidden inline-block bg-neutral-950/60 w-full rounded-b-md transition-all duration-200">
		<ul class="flex flex-col space-y-2 text-right mr-4">
			{#each links as link}
				<li>
					<a href="{link.url}" class="block py-2 hover:text-purple-400">{link.text}</a>
				</li>
			{/each}
		</ul>
	</div>
{/if}
