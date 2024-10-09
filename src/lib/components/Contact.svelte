<section id="contact" class="py-12 mx-1">
	<h3 class="text-center text-3xl font-bold mb-6">Contact Us</h3>
	<div
		class="max-w-7xl mx-auto grid grid-cols-1 justify-items-center gap-8 mb-10"
	>
		<div
			class="w-full max-w-sm sm:max-w-lg md:max-w-2xl lg:max-w-4xl flex flex-col group relative overflow-hidden rounded-xl px-4 py-5 shadow-[0_1000px_0_0_hsl(0_0%_20%)_inset] transition-colors duration-200 flex-grow"
		>
			<span
				class="backdrop absolute inset-px rounded-[11px] bg-neutral-950 transition-colors duration-200"
			></span>

			<div
				class="z-10 grid grid-cols-1 lg:grid-cols-2 lg:justify-items-end w-full"
			>
				<div class="space-y-2 ml-4 mb-6">
					<p class="text-xl font-semibold">Online Support</p>
					<p>
						Still have a question? Want to request a trial? Send us
						a message.
					</p>
				</div>
				<div class="mr-4 grid place-items-center">
					<a href="https://wa.me/15551234567">
						<button
							class="group relative grid overflow-hidden rounded-xl px-4 py-2 my-auto shadow-[0_1000px_0_0_hsl(0_0%_50%)_inset] transition-colors duration-200"
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
								class="z-10 text-sm font-medium relative after:absolute after:bg-neutral-400 after:bottom-0 after:left-0 after:h-px after:w-full after:origin-bottom-right after:scale-x-0 hover:after:origin-bottom-left hover:after:scale-x-100 after:transition-transform after:ease-in-out after:duration-300"
							>
								<slot>Whatsapp</slot>
							</span>
						</button>
					</a>
				</div>
			</div>
		</div>
	</div>
</section>
