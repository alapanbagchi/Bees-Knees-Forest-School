<script>
	import Button from '$lib/components/Button.svelte';
	import FeaturesCard from '$lib/components/FeaturesCard.svelte';
	import Accordian from '$lib/components/Accordian.svelte';
	const features = [
		{
			name: 'Risk Assessment',
			description:
				'We encourage kids to make their own risk assessments with minimal adult interference which allows children the space and time to develop natural problem solving skills. We foster a sense of responsibility and judgement that can benefit them in various aspects of life.',
			image:
				'https://cdn.discordapp.com/attachments/1020025379840327741/1160136628048769034/anarkyyy_Adventurous_kids_showing_risk_assessment_skills_in_eng_e6aba248-cebd-4ada-9315-3086fa945e58.png?ex=653ccaee&is=652a55ee&hm=ef959e8b424f1b08be960235ef3cad1f109f9e8858afeaa22a9ecc5dd2e1651a&'
		},
		{
			name: 'Curiosity and Learning',
			description:
				'By nurturing curiosity, our clubs help children become curious learners for life, promoting a thirst for knowledge that goes beyond the classroom.',
			image:
				'https://cdn.discordapp.com/attachments/1020025379840327741/1160136628048769034/anarkyyy_Adventurous_kids_showing_risk_assessment_skills_in_eng_e6aba248-cebd-4ada-9315-3086fa945e58.png?ex=653ccaee&is=652a55ee&hm=ef959e8b424f1b08be960235ef3cad1f109f9e8858afeaa22a9ecc5dd2e1651a&'
		},
		{
			name: 'Physical Development',
			description:
				'Our clubs support the development of stronger physical abilities in children through outdoor activities, promoting health and well-being.',
			image:
				'https://cdn.discordapp.com/attachments/1020025379840327741/1160136628048769034/anarkyyy_Adventurous_kids_showing_risk_assessment_skills_in_eng_e6aba248-cebd-4ada-9315-3086fa945e58.png?ex=653ccaee&is=652a55ee&hm=ef959e8b424f1b08be960235ef3cad1f109f9e8858afeaa22a9ecc5dd2e1651a&'
		},
		{
			name: 'Emotional Resilience',
			description:
				'The outdoor setting allows children to develop emotional resilience by navigating the challenges and uncertainties of the natural world, helping them build inner strength.',
			image:
				'https://cdn.discordapp.com/attachments/1020025379840327741/1160136628048769034/anarkyyy_Adventurous_kids_showing_risk_assessment_skills_in_eng_e6aba248-cebd-4ada-9315-3086fa945e58.png?ex=653ccaee&is=652a55ee&hm=ef959e8b424f1b08be960235ef3cad1f109f9e8858afeaa22a9ecc5dd2e1651a&'
		},

		{
			name: 'Effective Communication',
			description:
				'Children attending our clubs become more effective communicators as they learn to express themselves in a diverse and interactive outdoor environment, improving their social skills.',
			image:
				'https://cdn.discordapp.com/attachments/1020025379840327741/1160136628048769034/anarkyyy_Adventurous_kids_showing_risk_assessment_skills_in_eng_e6aba248-cebd-4ada-9315-3086fa945e58.png?ex=653ccaee&is=652a55ee&hm=ef959e8b424f1b08be960235ef3cad1f109f9e8858afeaa22a9ecc5dd2e1651a&'
		},
		{
			name: 'Self-Confidence',
			description:
				'Participation in our clubs can boost a childs self-confidence, as they conquer outdoor challenges and gain a sense of accomplishment.',
			image:
				'https://cdn.discordapp.com/attachments/1020025379840327741/1160136628048769034/anarkyyy_Adventurous_kids_showing_risk_assessment_skills_in_eng_e6aba248-cebd-4ada-9315-3086fa945e58.png?ex=653ccaee&is=652a55ee&hm=ef959e8b424f1b08be960235ef3cad1f109f9e8858afeaa22a9ecc5dd2e1651a&'
		},
		{
			name: 'Sensory Learning',
			description:
				'Our approach and clubs engage childrens senses - research has proven that information acquired through the use of all our senses leads to knowledge being ingrained rather than simply retained for a short period of time.',
			image:
				'https://cdn.discordapp.com/attachments/1020025379840327741/1160136628048769034/anarkyyy_Adventurous_kids_showing_risk_assessment_skills_in_eng_e6aba248-cebd-4ada-9315-3086fa945e58.png?ex=653ccaee&is=652a55ee&hm=ef959e8b424f1b08be960235ef3cad1f109f9e8858afeaa22a9ecc5dd2e1651a&'
		},
		{
			name: 'Learning Through Play',
			description:
				'Our approach emphasises learning through play, which helps children engage with their environment in a fun and meaningful way, promoting a positive attitude toward learning in all stages of life',
			image:
				'https://cdn.discordapp.com/attachments/1020025379840327741/1160136628048769034/anarkyyy_Adventurous_kids_showing_risk_assessment_skills_in_eng_e6aba248-cebd-4ada-9315-3086fa945e58.png?ex=653ccaee&is=652a55ee&hm=ef959e8b424f1b08be960235ef3cad1f109f9e8858afeaa22a9ecc5dd2e1651a&'
		},
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
			<h1 class="max-md:text-3xl text-5xl leading-[50px] -mb-3">The best after school club for your kids</h1>
			<p class="max-md:w-full w-3/5 leading-7 opacity-90">
				Lorem ipsum dolor sit amet consectetur, adipisicing elit. Officia eaque inventore veniam
				minus dicta corrupti rerum nihil! Voluptas tempora similique odit! Reprehenderit ipsam
				doloribus sapiente, facere ipsum magni perferendis nostrum!
			</p>
			<div>
				<Button classname="flex items-center " variant="WHITE"
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
	<h2 class="max-md:text-2xl max-md:leading-[35px] text-3xl leading-[50px] text-primary my-6">Why our clubs are the bee's knees</h2>
	<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 h-full gap-5 ">
		{#each features as feature}
			<FeaturesCard title={feature.name} description={feature.description} image={feature.image} />
		{/each}
	</div>
</section>
<section id="faq" class="container h-full">
	<h2 class="max-md:text-2xl max-md:leading-[35px] text-3xl leading-[50px] text-primary my-6">Frequently Asked Questions</h2>
	<div class="grid grid-cols-2 max-md:grid-cols-1 h-full gap-5">
		{#each features as feature}
			<Accordian title={feature.name} content={feature.description} />
		{/each}
	</div>
</section>