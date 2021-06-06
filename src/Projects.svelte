<script>
	import gms from "./assets/gms.png";
	import box from "./assets/box.png";
	import kaktus from "./assets/kaktus.png";
	import pac3 from "./assets/pac3.png";
	import inzy from "./assets/inzy.png";
	import vitals from "./assets/vitals.png";
	import Card from "./lib/Card.svelte";
	import Navbar from "./lib/Navbar.svelte";
	import Footer from "./lib/Footer.svelte";
</script>

<Navbar />
<div class="flex flex-col">
	<main class="bg-gray-900">
		<div class="mt-12 max-w-7xl mx-auto grid gap-5 lg:grid-cols-3">
			<Card src={inzy} tags={["Svelte", "Tailwind", "JS"]}>
				<span slot="title"
					><a href="/" target="_blank" class="hover:text-gray-300"
						>📝 Portfolio</a
					></span
				>
				<span slot="desc"
					>This portfolio was created in order to polish my svelte and tailwind
					skills as also to show off my current and past projects.</span
				>
			</Card>
			<Card src={box} tags={["Unity", "C#"]}>
				<span slot="title"
					><a
						href="https://gamejolt.com/games/StrangeBoxes/483189"
						target="_blank"
						class="hover:text-gray-300">📦 Strange Boxes</a
					></span
				>
				<span slot="desc"
					>Quick tetris like game, created for gamejam organised and sponsored
					by Polish goverment.</span
				>
			</Card>
			<Card src={gms} tags={["Node.js", "Discord.js"]}>
				<span slot="title">🤖 GMSBot</span>
				<span slot="desc"
					>Discord bot that scrapes gmodstore jobs page for existing listings
					and sends message with details about new ones.</span
				>
			</Card>
			<Card src={kaktus} tags={["Lua"]}>
				<span slot="title"
					><a
						href="https://forum.kaktusownia.com.pl/"
						class="hover:text-gray-300"
						target="_blank">Kaktusownia Dev</a
					></span
				>
				<span slot="desc"
					>Kaktusownia is the biggest Garry's Mod community in Poland that runs
					multiple servers based on roleplaying gamemodes. Worked on countless
					smaller projects during my stay as a developer.
				</span>
			</Card>
			<Card src={vitals} tags={["Lua"]}>
				<span slot="title">zMedic</span>
				<span slot="desc">
					zMedic is a script created for German community Pryers.de, that
					included dedicated limb system, vital signs board and etc.
				</span>
			</Card>
			<Card src={pac3} tags={["Python", "Regex"]}>
				<span slot="title">PAC3 Parser</span>
				<span slot="desc">
					PAC3 pose parser to EGM Animation SWEP base made in order to acquire
					fast and easy pose creation for roleplay purposes.
				</span>
			</Card>
		</div>
	</main>
</div>
<Footer />
