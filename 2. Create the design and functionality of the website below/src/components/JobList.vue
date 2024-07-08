<script setup>
import JobItem from "./JobItem.vue";
import { ref } from "vue";
import { FwbButton, FwbModal } from "flowbite-vue";

const isShowModal = ref(false);
const currentJobShown = ref(null);

function closeModal() {
	isShowModal.value = false;
}
function showModal() {
	isShowModal.value = true;
}

const jobs = [
	{
		title: "Marketing Planner",
		jobDescriptions: [
			"Monitor competition to identify new industry trends and opportunities for innovation",
			"Develop marketing strategies based on customer preferences, business objectives, and available resources",
			"Conduct market research to identify potential customers and assess their needs, interests, and preferences",
			"Work with design teams to develop marketing materials such as brochures, ads, and presentations",
			"Create an advertising budget that reflects the company’s priorities while remaining within the parameters set by upper management",
			"Develop an effective communications strategy for each campaign using several different channels, including social media, email, push notification, print ads",
			"Create a detailed timeline of all marketing activities, including production schedules, deadlines for materials delivery, and event dates and locations",
			"Provide feedback to superiors regarding the effectiveness of new campaigns and recommend adjustments",
		],
		skills: [
			"Minimum bachelor degree in Marketing Management;",
			"Minimum 3-5 years experience as Marketing Manager/Director in any marketplace industry;",
			"Good time management and project management skill;",
			"Creative communication skill in both verbal and design",
			"Multi-language abilities in verbal and non-verbal",
		],
	},
	{
		title: "Marketing Planner",
		jobDescriptions: [
			"Monitor competition to identify new industry trends and opportunities for innovation",
			"Develop marketing strategies based on customer preferences, business objectives, and available resources",
			"Conduct market research to identify potential customers and assess their needs, interests, and preferences",
			"Work with design teams to develop marketing materials such as brochures, ads, and presentations",
			"Create an advertising budget that reflects the company’s priorities while remaining within the parameters set by upper management",
			"Develop an effective communications strategy for each campaign using several different channels, including social media, email, push notification, print ads",
			"Create a detailed timeline of all marketing activities, including production schedules, deadlines for materials delivery, and event dates and locations",
			"Provide feedback to superiors regarding the effectiveness of new campaigns and recommend adjustments",
		],
		skills: [
			"Minimum bachelor degree in Marketing Management;",
			"Minimum 3-5 years experience as Marketing Manager/Director in any marketplace industry;",
			"Good time management and project management skill;",
			"Creative communication skill in both verbal and design",
			"Multi-language abilities in verbal and non-verbal",
		],
	},
	{
		title: "Marketing Planner",
		jobDescriptions: [
			"Monitor competition to identify new industry trends and opportunities for innovation",
			"Develop marketing strategies based on customer preferences, business objectives, and available resources",
			"Conduct market research to identify potential customers and assess their needs, interests, and preferences",
			"Work with design teams to develop marketing materials such as brochures, ads, and presentations",
			"Create an advertising budget that reflects the company’s priorities while remaining within the parameters set by upper management",
			"Develop an effective communications strategy for each campaign using several different channels, including social media, email, push notification, print ads",
			"Create a detailed timeline of all marketing activities, including production schedules, deadlines for materials delivery, and event dates and locations",
			"Provide feedback to superiors regarding the effectiveness of new campaigns and recommend adjustments",
		],
		skills: [
			"Minimum bachelor degree in Marketing Management;",
			"Minimum 3-5 years experience as Marketing Manager/Director in any marketplace industry;",
			"Good time management and project management skill;",
			"Creative communication skill in both verbal and design",
			"Multi-language abilities in verbal and non-verbal",
		],
	},
	{
		title: "Marketing Planner",
		jobDescriptions: [
			"Monitor competition to identify new industry trends and opportunities for innovation",
			"Develop marketing strategies based on customer preferences, business objectives, and available resources",
			"Conduct market research to identify potential customers and assess their needs, interests, and preferences",
			"Work with design teams to develop marketing materials such as brochures, ads, and presentations",
			"Create an advertising budget that reflects the company’s priorities while remaining within the parameters set by upper management",
			"Develop an effective communications strategy for each campaign using several different channels, including social media, email, push notification, print ads",
			"Create a detailed timeline of all marketing activities, including production schedules, deadlines for materials delivery, and event dates and locations",
			"Provide feedback to superiors regarding the effectiveness of new campaigns and recommend adjustments",
		],
		skills: [
			"Minimum bachelor degree in Marketing Management;",
			"Minimum 3-5 years experience as Marketing Manager/Director in any marketplace industry;",
			"Good time management and project management skill;",
			"Creative communication skill in both verbal and design",
			"Multi-language abilities in verbal and non-verbal",
		],
	},
	{
		title: "Marketing Planner",
		jobDescriptions: [
			"Monitor competition to identify new industry trends and opportunities for innovation",
			"Develop marketing strategies based on customer preferences, business objectives, and available resources",
			"Conduct market research to identify potential customers and assess their needs, interests, and preferences",
			"Work with design teams to develop marketing materials such as brochures, ads, and presentations",
			"Create an advertising budget that reflects the company’s priorities while remaining within the parameters set by upper management",
			"Develop an effective communications strategy for each campaign using several different channels, including social media, email, push notification, print ads",
			"Create a detailed timeline of all marketing activities, including production schedules, deadlines for materials delivery, and event dates and locations",
			"Provide feedback to superiors regarding the effectiveness of new campaigns and recommend adjustments",
		],
		skills: [
			"Minimum bachelor degree in Marketing Management;",
			"Minimum 3-5 years experience as Marketing Manager/Director in any marketplace industry;",
			"Good time management and project management skill;",
			"Creative communication skill in both verbal and design",
			"Multi-language abilities in verbal and non-verbal",
		],
	},
	{
		title: "Marketing Planner",
		jobDescriptions: [
			"Monitor competition to identify new industry trends and opportunities for innovation",
			"Develop marketing strategies based on customer preferences, business objectives, and available resources",
			"Conduct market research to identify potential customers and assess their needs, interests, and preferences",
			"Work with design teams to develop marketing materials such as brochures, ads, and presentations",
			"Create an advertising budget that reflects the company’s priorities while remaining within the parameters set by upper management",
			"Develop an effective communications strategy for each campaign using several different channels, including social media, email, push notification, print ads",
			"Create a detailed timeline of all marketing activities, including production schedules, deadlines for materials delivery, and event dates and locations",
			"Provide feedback to superiors regarding the effectiveness of new campaigns and recommend adjustments",
		],
		skills: [
			"Minimum bachelor degree in Marketing Management;",
			"Minimum 3-5 years experience as Marketing Manager/Director in any marketplace industry;",
			"Good time management and project management skill;",
			"Creative communication skill in both verbal and design",
			"Multi-language abilities in verbal and non-verbal",
		],
	},
];

function onSeeJobClicked(job) {
	return () => {
		console.log("onSeeJobClicked", job.title);
		showModal();
		currentJobShown.value = job;
	};
}
</script>

<template>
	<div class="joblist">
		<JobItem :onSeeJobClicked="onSeeJobClicked(job)" v-for="job in jobs">
			<template #jobTitle>Marketing Planner</template>
		</JobItem>
	</div>

	<fwb-modal size="6xl" v-if="isShowModal" @close="closeModal">
		<template #header> </template>
		<template #body>
			<div class="px-[3rem] pb-[1rem]">
				<p class="text-[#4b9741] text-[2rem] font-bold mb-4">
					{{ currentJobShown.title }}
				</p>
				<h5 class="mb-2 text-xl [font-weight:bolder]">Job Description :</h5>
				<ul class="mb-4 list-disc list-item list-outside">
					<li v-for="jobDescription in currentJobShown.jobDescriptions">
						{{ jobDescription }}
					</li>
				</ul>
				<h5 class="mb-2 text-xl [font-weight:bolder]">Skill :</h5>
				<ul class="mb-4 list-disc list-item list-outside">
					<li v-for="skill in currentJobShown.skills">
						{{ skill }}
					</li>
				</ul>
				<h1 class="text-xl font-bold pt-6 pb-4">Send Your Job Application</h1>
			</div>
		</template>
		<template #footer>
			<div class="flex justify-between">
				<fwb-button @click="closeModal" color="alternative">
					Decline
				</fwb-button>
				<fwb-button @click="closeModal" color="green"> I accept </fwb-button>
			</div>
		</template>
	</fwb-modal>
</template>

<style scoped>
.joblist {
	display: grid;
	grid-template-columns: 1fr;
	row-gap: 1rem;
	column-gap: 2rem;
	padding: 1rem;
}
@media screen and (min-width: 768px) {
	.joblist {
		grid-template-columns: 1fr 1fr;
	}
}
</style>
