<script>
	import Android from "./svg/Android.svelte";
	import Apple from "./svg/Apple.svelte";
	import Laptop from "./svg/Laptop.svelte";
	import SmartTV from "./svg/SmartTV.svelte";
	import Windows from "./svg/Windows.svelte";
</script>

<!-- Add background image -->
<section
	class="text-center pb-16 relative py-8 md:py-16 lg:py-24 mx-1"
	id="home"
	style="overflow: hidden; min-height: 500px;"
>
	<div
		class="absolute inset-0 bg-cover bg-center bg-no-repeat bg-fixed"
		style="background-image: url('/iptv.jpg'); filter: brightness(0.5);"
	></div>
	<div class="relative z-10 container mx-auto px-4 lg:py-12">
		<h1
			class="text-5xl font-bold mb-6 leading-tight tracking-wide text-shadow-lg lg:text-6xl"
		>
			Best IPTV Subscription
		</h1>
		<p
			class="mt-4 text-xl leading-relaxed max-w-2xl mx-auto text-shadow-md lg:text-2xl"
		>
			Enjoy excellent image quality up to 4K on any device, with over
			20,000 channels and 150,000 videos on demand.100% uptime with our
			best IPTV subscription!
		</p>

		<div class="flex justify-center mt-12 lg:mt-16 space-x-4 lg:space-x-6">
			<div
				class="h-12 w-12 object-contain transition-transform hover:scale-110 mr-2 lg:h-16 lg:w-16"
			>
				<SmartTV></SmartTV>
				<p>Smart TV</p>
			</div>
			<div
				class="h-12 w-12 object-contain transition-transform hover:scale-110 lg:h-16 lg:w-16"
			>
				<Laptop />
				<p>Laptop</p>
			</div>
			<div
				class="h-12 w-12 object-contain transition-transform hover:scale-110 lg:h-16 lg:w-16"
			>
				<Android />
				<p class="text-right">Android</p>
			</div>
			<div
				class="h-12 w-12 object-contain transition-transform hover:scale-110 lg:h-16 lg:w-16"
			>
				<Apple />
				<p class="text-center">iOS</p>
			</div>
			<div
				class="h-12 w-12 object-contain transition-transform hover:scale-110 lg:h-16 lg:w-16"
			>
				<Windows />
				<p>Windows</p>
			</div>
		</div>
	</div>
</section>
