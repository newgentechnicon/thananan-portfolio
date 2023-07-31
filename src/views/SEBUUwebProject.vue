<script>
import feather from 'feather-icons';
import ProjectHeader from '../components/projects/ProjectHeader.vue';
import ProjectGallery from '../components/projects/ProjectGallery.vue';
import ProjectInfo from '../components/projects/ProjectInfo.vue';
// import ProjectRelatedProjects from '../components/projects/ProjectRelatedProjects.vue';

export default {
	name: 'Projects',
	components: {
		ProjectHeader,
		ProjectGallery,
		ProjectInfo,
		// ProjectRelatedProjects,
	},
	data: () => {
		return {
			singleProjectHeader: {
				singleProjectTitle: 'SE BUU Website',
				singleProjectDate: 'Mar 16, 2020',
				singleProjectTag: 'SA / UI / Frontend / QA',
			},
			projectImages: [
				{
					id: 1,
					title: 'Kabul Project Management UI',
					img: require('@/assets/images/project/sebuu/SEBUU-project-1.png'),
				},
				{
					id: 2,
					title: 'Kabul Project Management UI',
					img: require('@/assets/images/project/sebuu/SEBUU-project-2.png'),
				},
				{
					id: 3,
					title: 'Kabul Project Management UI',
					img: require('@/assets/images/project/sebuu/SEBUU-project-3.png'),
				},
			],
			projectInfo: {
				clientHeading: 'About Client',
				companyInfos: [
					{
						id: 1,
						title: 'Name',
						details: 'Software Engineer Major, Burapha University',
					},
					{
						id: 2,
						title: 'Services',
						details: 'Software Design, UI Design, Frontend Development, Quality Assurance',
					},
					// {
					// 	id: 3,
					// 	title: 'Website',
					// 	details: 'https://company.com',
					// },
					{
						id: 3,
						title: 'Phone',
						details: '+66 038 103 096',
					},
				],
				objectivesHeading: 'Objective',
				objectivesDetails:
					'Implements the application by Design software by UML, Implements web application, and test system.',
				technologies: [
					{
						title: 'Tools & Technologies',
						techs: [
							'HTML',
							'CSS',
							'JavaScript',
							'PHP',
							'Codeigniter',
							'Bootstrap',
							'Adobe Illustrator',
							'Scrum Model',
						],
					},
				],
				projectDetailsHeading: 'Challenge',
				projectDetails: [
					{
						id: 1,
						details:
							'Lecturer in Software Engineering Saw the implementation of information systems in the Information Systems Engineering Laboratory (ISERL) to be adapted to suit educational administration to see the overall picture within the organization. The project administrators then applied the management system in the software engineering department, Burapha University. That integrates Human resource management system, register and processing of studies system, and Students affairs officers system, etc. In this project implementation was created to be integrated with the 5 main missions of higher education institutions consisting of manufacturing graduates, research, academic services, Art and culture support, and business administration. Which helps the teacher can handle education information view education and personnel information reports within the organization. To plan for management, and for maximum efficiency. There is also a section of Smart Web that was developed for general users. Who want to know new news Able to be informed of software engineering programs The system has been accepted by teachers in the software engineering department. And there are plans for further development and future applications in software engineering.',
					},
					{
						id: 1,
						details:
							'Integrating different databases from an existing educational system poses a significant challenge due to the variations in the systems. Bringing all these systems together to ensure seamless data integration is a complex task.',
					},
					{
						id: 2,
						details:
							'In this project, I have developed several websites, including a Landing page and a website for accessing information about the field of software engineering at Burapha University. As part of the development, an additional display screen has also been designed.',
					},
					{
						id: 3,
						details:
							'The system has been meticulously designed using UML documents, ensuring that it can be developed and easily extended in the future. Furthermore, comprehensive system testing has been conducted prior to delivery to minimize any potential errors in the final product.',
					},
				],
				socialSharingsHeading: 'Share This',
				socialSharings: [
					{
						id: 1,
						name: 'Twitter',
						icon: 'twitter',
						url: 'https://twitter.com/',
					},
					{
						id: 2,
						name: 'Instagram',
						icon: 'instagram',
						url: 'https://instagram.com/',
					},
					{
						id: 3,
						name: 'Facebook',
						icon: 'facebook',
						url: 'https://facebook.com/',
					},
					{
						id: 4,
						name: 'LinkedIn',
						icon: 'linkedin',
						url: 'https://linkedin.com/',
					},
					{
						id: 5,
						name: 'Youtube',
						icon: 'youtube',
						url: 'https://www.youtube.com/',
					},
				],
			},
			// relatedProject: {
			// 	relatedProjectsHeading: 'Related Projects',
			// 	relatedProjects: [
			// 		{
			// 			id: 1,
			// 			title: 'Mobile UI',
			// 			img: require('@/assets/images/mobile-project-1.jpg'),
			// 		},
			// 		{
			// 			id: 2,
			// 			title: 'Web Application',
			// 			img: require('@/assets/images/web-project-1.jpg'),
			// 		},
			// 		{
			// 			id: 3,
			// 			title: 'UI Design',
			// 			img: require('@/assets/images/ui-project-2.jpg'),
			// 		},
			// 		{
			// 			id: 4,
			// 			title: 'Kabul Mobile App UI',
			// 			img: require('@/assets/images/mobile-project-2.jpg'),
			// 		},
			// 	],
			// },
		};
	},
	mounted() {
		feather.replace();
	},
	updated() {
		feather.replace();
	},
	methods: {},
};
</script>

<template>
	<div class="container mx-auto mt-10 sm:mt-20">
		<!-- Project header -->
		<ProjectHeader :singleProjectHeader="singleProjectHeader" />

		<!-- Project gallery -->
		<ProjectGallery :projectImages="projectImages" />

		<!-- Project information -->
		<ProjectInfo :projectInfo="projectInfo" />

		<!-- Project related projects -->
		<!-- <ProjectRelatedProjects :relatedProject="relatedProject" /> -->
	</div>
</template>

<style scoped></style>
