<script>
	import Button from '$lib/components/Button.svelte';
	import FeaturesCard from '$lib/components/FeaturesCard.svelte';
	import Accordian from '$lib/components/Accordian.svelte';
	import { FAQ } from '../data/faq';
	import Input from '$lib/components/ui/Input/Input.svelte';
	const features = [
		{
			name: 'Risk Assessment',
			description:
				'We encourage kids to make their own risk assessments with minimal adult interference which allows children the space and time to develop natural problem solving skills. We foster a sense of responsibility and judgement that can benefit them in various aspects of life.',
			image: 'https://cdn.midjourney.com/3acad77c-0d08-41c0-be4c-df59ee102322/0_1.webp'
		},
		{
			name: 'Curiosity and Learning',
			description:
				'By nurturing curiosity, our clubs help children become curious learners for life, promoting a thirst for knowledge that goes beyond the classroom.',
			image: 'https://cdn.midjourney.com/1334ccf7-2026-49de-b0ec-57612c47a4de/0_1.webp'
		},
		{
			name: 'Physical Development',
			description:
				'Our clubs support the development of stronger physical abilities in children through outdoor activities, promoting health and well-being.',
			image: 'https://cdn.midjourney.com/1259a882-c70c-444d-91e0-413fac57073e/0_3.webp'
		},
		{
			name: 'Emotional Resilience',
			description:
				'The outdoor setting allows children to develop emotional resilience by navigating the challenges and uncertainties of the natural world, helping them build inner strength.',
			image: 'https://cdn.midjourney.com/eac06a5c-62f8-446f-845a-6556c820ede0/0_0.webp'
		},

		{
			name: 'Effective Communication',
			description:
				'Children attending our clubs become more effective communicators as they learn to express themselves in a diverse and interactive outdoor environment, improving their social skills.',
			image: 'https://cdn.midjourney.com/dd1f6e4f-e47e-4088-88f5-27fa7c272aa5/0_2.webp'
		},
		{
			name: 'Self-Confidence',
			description:
				'Participation in our clubs can boost a childs self-confidence, as they conquer outdoor challenges and gain a sense of accomplishment.',
			image: 'https://cdn.midjourney.com/cb9d7681-96a9-42d9-9543-a6b340313f53/0_1.webp'
		},
		{
			name: 'Sensory Learning',
			description:
				'Our approach and clubs engage childrens senses - research has proven that information acquired through the use of all our senses leads to knowledge being ingrained rather than simply retained for a short period of time.',
			image: 'https://cdn.midjourney.com/a4b45a20-90fe-464f-9b5c-df39ece1faf6/0_3.webp'
		},
		{
			name: 'Learning Through Play',
			description:
				'Our approach emphasises learning through play, which helps children engage with their environment in a fun and meaningful way, promoting a positive attitude toward learning in all stages of life',
			image: 'https://cdn.midjourney.com/50793d7b-576d-4cb6-8f68-7b75f74c9c92/0_3.webp'
		}
	];
</script>

<section class="h-[80vh] relative overflow-hidden z-0">
	<div class="w-full h-full overflow-hidden">
		<img
			src="https://cdn.discordapp.com/attachments/1020025379840327741/1159805988778541156/anarkyyy_bright_sun_shines_through_a_woods._in_the_style_of_nat_44860b68-629b-4417-ac5a-2d12d3904c10.png?ex=653b96ff&is=652921ff&hm=feb2cdc56013d94f75a02d7878fbd8ae4deaf3e3b90b027c0edd93d619cf939d&"
			alt=""
			class="w-full h-full object-cover"
		/>
		<div class="absolute top-0 z-10 bg-black/50 h-[100vh] w-full transition-all" />
	</div>
	<div class="w-full h-full flex items-center absolute top-0 text-white z-10">
		<div class="container ml-auto flex flex-col gap-7">
			<h1 class="max-md:text-3xl text-5xl font-bold leading-[50px] -mb-3 text-center">
				Rooted in Fun, Growing in Nature
			</h1>
			<p class="max-md:w-full w-3/5 leading-7 opacity-90 text-center mx-auto">
				The Bee's Knees Forest School - providing immersive outdoor learning experiences that
				empower children to discover, explore, and learn in the heart of nature, fostering
				creativity, resilience, and a lifelong love for the environment.
			</p>
			<div>
				<Button classname="flex items-center mx-auto" variant="WHITE"
					><svg
						width="30"
						height="30"
						viewBox="0 0 54 54"
						fill="none"
						xmlns="http://www.w3.org/2000/svg"
					>
						<path
							d="M26.8555 0.962967C12.2162 0.962967 0.335205 12.6276 0.335205 27C0.335205 41.3724 12.2162 53.037 26.8555 53.037C41.4946 53.037 53.3757 41.3724 53.3757 27C53.3757 12.6276 41.5212 0.962967 26.8555 0.962967ZM34.8116 32.8063L27.1204 37.1544C26.1657 37.7012 25.1052 37.9616 24.0706 37.9616C23.0101 37.9616 21.9755 37.7012 21.0209 37.1544C19.1115 36.0609 17.9711 34.1342 17.9711 31.947V23.2246C17.9711 21.0636 19.1115 19.1108 21.0209 18.0172C22.9305 16.9237 25.211 16.9237 27.147 18.0172L34.8378 22.3654C36.7473 23.459 37.8876 25.3857 37.8876 27.5728C37.8876 29.7599 36.7473 31.7127 34.8116 32.8063Z"
							fill="#292D32"
						/>
					</svg>
					<p class="px-3">See More</p>
				</Button>
			</div>
		</div>
	</div>
</section>
<section class="container h-full">
	<h2
		class="max-md:text-2xl max-md:leading-[35px] text-3xl leading-[50px] my-8 text-center text-[#CF572B] font-semibold"
	>
		Why our clubs are the Bee's Knees
	</h2>
	<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 h-full gap-5">
		{#each features as feature}
			<FeaturesCard title={feature.name} description={feature.description} image={feature.image} />
		{/each}
	</div>
	<div class="w-full mt-8 flex justify-center">
		<a href="/clubs">
			<Button variant="RED" classname="font-semibold">See Our Clubs</Button>
		</a>
	</div>
</section>
<section id="faq" class="container h-full">
	<h2
		class="max-md:text-2xl max-md:leading-[35px] text-3xl leading-[50px] text-[#CF572B] font-semibold my-8 text-center"
	>
		Frequently Asked Questions
	</h2>
	<div class="grid grid-cols-2 max-md:grid-cols-1 h-full gap-5">
		{#each FAQ as faq}
			<Accordian title={faq.question} content={faq.answer} />
		{/each}
	</div>
</section>

<section class="mt-12 container">
	<div
		class="bg-[#DAE69F] flex flex-col space-y justify-center w-full rounded-xl h-[300px] max-md:h-fit text-center space-y-2"
	>
		<div
			class="w-[70%] max-md:w-[100%] max-md:px-4 max-md:py-10
		mx-auto space-y-3"
		>
			<h2 class="max-md:text-2xl text-3xl text-[#374b35]">
				Subscribe to Bee's Knees Forest School
			</h2>
			<p class="max-md:text-sm opacity-80 leading-6">
				Join our newsletter and receive the latest news, tips, and exclusive offers directly in your
				inbox. Enter your email below and hit subscribe now!
			</p>
			<div class="flex gap-4 max-md:flex-col max-md:gap-2">
				<Input class="border-[#374b35]" placeholder="Enter your email" />
				<Button variant="PRIMARY">Subscribe</Button>
			</div>
		</div>
	</div>
</section>
