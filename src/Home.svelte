<script>
	import Gif from "./assets/prof.gif";
	import Footer from "./lib/Footer.svelte";
	import Navbar from "./lib/Navbar.svelte";
</script>

<div class="flex flex-col h-screen">
	<Navbar />
	<div class="bg-gray-900 flex-grow grid place-items-center">
		<div class="mx-auto max-w-7xl">
			<div class="lg:grid lg:grid-cols-12 lg:gap-8">
				<div
					class="px-4 sm:px-6 sm:text-center md:max-w-2xl md:mx-auto lg:col-span-6 lg:text-left lg:flex lg:items-center"
				>
					<div>
						<h1
							class="mt-4 text-4xl tracking-tight font-extrabold text-white sm:mt-5 sm:leading-none lg:mt-6 lg:text-5xl xl:text-6xl"
						>
							<span class="md:block text-blue-500">zgredinzyyy</span>
						</h1>
						<p
							class="mt-3 text-base text-gray-100 sm:mt-5 sm:text-xl lg:text-lg xl:text-xl"
						>
							<span class="lg:text-2xl xl:text-3xl font-semibold">Hi!</span> I'm
							Bartosh, 18 year old software developer, cybersecurity enthusiast who
							likes to explore new technologies and discover their maximum capabilities.
						</p>
					</div>
				</div>
				<div
					class="mt-16 sm:mt-24 grid place-items-center lg:block lg:mt-0 lg:col-span-6"
				>
					<img
						class="inline-block max-h-80 rounded-full lg:ml-20"
						src={Gif}
						alt=""
					/>
				</div>
			</div>
		</div>
	</div>
</div>
<Footer />
