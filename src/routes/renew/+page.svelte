<svelte:head>
	<title>Renew | NetStreamHub</title>
</svelte:head>

<div class="w-full">
	<section
		id="renew"
		class="py-12 mx-1"
		style="overflow: hidden; min-height: 500px;"
	>
		<h3 class="text-center text-3xl font-bold mb-6">IPTV Renew</h3>
		<div
			class="grid grid-cols-1 mx-auto gap-4 max-w-3xl justify-items-center w-full"
		>
			<div
				class="bg-neutral rounded-xl p-4 shadow-[0_1000px_0_0_hsl(0_0%_20%)_inset] transition-colors duration-200"
			>
				<div class="">
					<p class="text-xl font-semibold text-center my-2">
						Welcome to our IPTV Subscription Renew page!
					</p>
					<p class="text-justify my-2">
						We value your continued support and are excited to offer
						a seamless and convenient way for you to extend your
						IPTV subscription. Thank you for choosing us as your
						preferred IPTV provider, and we look forward to
						continuing to deliver high-quality entertainment to your
						screens. Stay connected and enjoy the best in streaming
						with our renewed subscription service!
					</p>
					<button
						class="group mx-auto mt-6 mb-4 relative grid overflow-hidden rounded-xl px-4 py-3 shadow-[0_1000px_0_0_hsl(0_0%_50%)_inset] transition-colors duration-200"
					>
						<span>
							<span
								class="spark mask-gradient animate-flip before:animate-kitrotate absolute inset-0 h-[100%] w-[100%] overflow-hidden rounded-xl [mask:linear-gradient(white,_transparent_50%)] before:absolute before:aspect-square before:w-[200%] before:rotate-[-90deg] before:bg-[conic-gradient(from_0deg,transparent_0_340deg,white_360deg)] before:content-[''] before:[inset:0_auto_auto_50%] before:[translate:-50%_-15%]"
							/>
						</span>
						<span
							class="backdrop absolute inset-px rounded-[11px] bg-purple-600 group-hover:bg-purple-800 transition-colors duration-200"
						/>
						<span
							class="z-10 text-lg font-semibold relative after:absolute after:bg-neutral-400 after:bottom-0 after:left-0 after:h-px after:w-full after:origin-bottom-right after:scale-x-0 hover:after:origin-bottom-left hover:after:scale-x-100 after:transition-transform after:ease-in-out after:duration-300"
						>
							<slot>Renew Now</slot>
						</span>
					</button>
					<a href="/#contact">
						<p class="text-center text-sm underline"> Still Having Trouble? Contact Us </p>
					</a>
				</div>
			</div>
		</div>
	</section>
</div>
