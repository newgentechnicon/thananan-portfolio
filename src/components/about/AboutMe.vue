<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						"Hello, I'am Thananan Thermsirisumsin (New). I have over 2 years of experience in writing web applications and mobile applications. Additionally, I have been working as a project manager for more than 1 year up to the present. I am also proficient in UX/UI, System design and Software testing.",
				},
				{
					id: 2,
					bio:
						'I strongly believe in delivering high-quality work that is closely aligned with customer needs. My approach involves working in an Agile style, drawing upon the skills I have accumulated throughout my work experience, to ensure the delivery of top-notch results that not only meet but also exceed customer expectations.',
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/profile.jpg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
