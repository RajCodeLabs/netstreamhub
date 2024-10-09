<script>
	const faq = [
		{
			question: "How can I test the IPTV service?",
			answer: `NetStreamHub IPTV offers one day free trial. With this you can watch all the channels, movies, and series available on our IPTV packages. Drop your email in the Trial Form, chat with us on <u><a href="https://wa.me/15551234567">WhatsApp</a></u>.`,
		},
		{
			question: "Available payment methods?",
			answer: "<ul><li>Credit / Debit Card (4% service fee)</li><li>Apple Pay (4% service fee)</li><li>Google Pay (4% service fee)</li><li>Cash App (4% service fee)</li><li>Cryptocurrency (BTC, LTC, ETH, USDT)</li></ul>",
		},
		{
			question: "Which devices can be used for IPTV?",
			answer: "Our IPTV services are accessible via all Smart TV devices (Samsung, Sony, LG…), all Android devices, Apple TV, iPhone, Google Chromecast, MAG box in the STB emulator app and FireStick.",
		},
		{
			question: "Recommended internet speed?",
			answer: "To watch all channels smoothly in the highest quality we recommend a minimum of 30 Mbps download speed. You can check your internet speed at <u><a href='https://fast.com'>https://fast.com</a></u>.",
		},
		{
			question: "Which countries are present?",
			answer: "Netherlands Belgium France UK Germany Switzerland Austria Poland Spain Malta Portugal Italy USA Canada Australia New Zealand Arabic India Pakistan Iran Turkey Azerbaycan Kurdistan Africa Afghanistan Armenia Exyu Slovenia Albania Greece Latino Brazil Caribbean Suriname Sweden Denmark Norway Finland Czech Bulgaria Romania Hungary Russia Georgia/Kazakh Ukraine Lithuania Latvia Estonia China/HK Malaysia Philippines Indonesia Korea Thailand Taiwan Vietnam Japan",
		},
		{
			question: "How many connections at once?",
			answer: "You may install your account on multiple devices, but keep in mind that it works on one at a time. We offer discounts for multi-connection lines, contact us for more details.",
		},
	];
</script>

<section class="py-12 mx-1" id="faq">
	<h3 class="text-center text-3xl font-bold mb-6">
		Frequently Asked Questions (FAQ)
	</h3>
	<div
		class="max-w-7xl mx-auto grid grid-cols-1 justify-items-center gap-8 mb-10"
	>
		{#each faq as { question, answer }}
			<div
				class="w-full max-w-sm sm:max-w-lg md:max-w-2xl lg:max-w-4xl flex flex-col"
			>
				<div
					class="group relative grid overflow-hidden rounded-xl px-4 py-5 shadow-[0_1000px_0_0_hsl(0_0%_20%)_inset] transition-colors duration-200 flex-grow"
				>
				
					<span
						class="backdrop absolute inset-px rounded-[11px] bg-neutral-950 transition-colors duration-200"
					></span>
					<div class="space-y-2 z-10">
						<details>
							<summary
								class="w-full text-left px-4 py-3 text-sm font-medium leading-5  hover:text-neutral-300 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-neutral-900 rounded-md transition-all duration-200 list-none"
							>
								<span class="flex items-center justify-between">
									<span class=" font-semibold"
										>{question}</span
									>
									<svg
										class="w-5 h-5 text-neutral-300 transition-transform duration-200"
										fill="none"
										stroke="currentColor"
										viewBox="0 0 24 24"
										xmlns="http://www.w3.org/2000/svg"
									>
										<path
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2"
											d="M19 9l-7 7-7-7"
										></path>
									</svg>
								</span>
							</summary>
							<div
								class="px-4 py-3 text-sm leading-5 text-neutral-400"
							>
								<p>{@html answer}</p>
							</div>
						</details>
					</div>
				</div>
			</div>
		{/each}
	</div>
</section>

<style>
	details[open] svg {
		transform: rotate(90deg);
		transition-property: transform;
	}
</style>
