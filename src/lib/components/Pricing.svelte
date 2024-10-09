<script>
	import Android from "./svg/Android.svelte";
import Apple from "./svg/Apple.svelte";
	import SmartTv from "./svg/SmartTV.svelte";
	import Windows from "./svg/Windows.svelte";

	let plans = [
		{
			duration: "24 months",
			price: 99.99,
			offerings: [
				"HD/FHD/4K IPTV",
				"+20K Live Channels",
				"+150K VOD",
				"Family Friendly",
				"TV Guide (EPG)",
			],
		},
		{
			duration: "12 months",
			price: 59.99,
			offerings: [
				"HD/FHD/4K IPTV",
				"+20K Live Channels",
				"+150K VOD",
				"Family Friendly",
				"TV Guide (EPG)",
			],
		},
		{
			duration: "6 months",
			price: 34.99,
			offerings: [
				"HD/FHD/4K IPTV",
				"+20K Live Channels",
				"+150K VOD",
				"Family Friendly",
				"TV Guide (EPG)",
			],
		},
		{
			duration: "3 months",
			price: 19.99,
			offerings: [
				"HD/FHD/4K IPTV",
				"+20K Live Channels",
				"+150K VOD",
				"Family Friendly",
				"TV Guide (EPG)",
			],
		},
		{
			duration: "1 month",
			price: 8.99,
			offerings: [
				"HD/FHD/4K IPTV",
				"+20K Live Channels",
				"+150K VOD",
				"Family Friendly",
				"TV Guide (EPG)",
			],
		},
	];
</script>

<section id="pricing" class=" py-12 mx-1">
	<h3 class="text-center text-3xl font-bold mb-6">Pricing</h3>
	<div
		class="max-w-6xl mx-auto justify-items-center  grid auto-rows-max grid-cols-1 md:grid-cols-3 lg:grid-cols-5 gap-4 mb-10"
	>
		{#each plans as plan}
		<div
			class="inline-flex animate-shine max-w-[350px] w-full items-center justify-center rounded-xl text-sm border border-white/10 bg-[linear-gradient(110deg,#000103,45%,#1e2631,55%,#000103)] bg-[length:200%_100%] px-4 py-5 transition-colors"
		>
		    <div class="flex flex-col gap-4">
				<p class="text-2xl font-semibold text-center text-neutral-200">{plan.duration}</p>

				<p class="text-5xl text-center font-semibold text-neutral-200">
                    ${plan.price}
                </p>
				<div class="text-sm flex flex-col">
					{#each plan.offerings as offering}
					<span> <b> ✓ </b> {offering} </span>
					<hr class=" border-neutral-700 mb-2" />
					{/each}
				</div>
				<button class="bg-purple-600 hover:bg-purple-800 text-white px-4 py-2 rounded-lg">Buy Now</button>
				<a href="/#contact" class="text-sm underline text-neutral-400">Having Trouble? Contact us</a>
				<div class="grid grid-cols-4 items-center place-items-center">
					<div class="h-5 w-5">
						<Apple />
					</div>
					<div class="h-5 w-5">
						<Android />
					</div>
					<div class=" ml-[1px] h-4 w-4">
						<Windows />
					</div>
					<div class="h-5 w-5">
						<SmartTv />
					</div>

				</div>
			</div>
		</div>
		{/each}
	</div>
</section>
