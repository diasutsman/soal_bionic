<script setup>
import JobItem from "./JobItem.vue";
</script>

<template>
	<div class="joblist">
		<JobItem>
			<template #jobTitle>Marketing Planner</template>
		</JobItem>
		<JobItem>
			<template #jobTitle>Marketing Planner</template>
		</JobItem>
		<JobItem>
			<template #jobTitle>Marketing Planner</template>
		</JobItem>
		<JobItem>
			<template #jobTitle>Marketing Planner</template>
		</JobItem>
		<JobItem>
			<template #jobTitle>Marketing Planner</template>
		</JobItem>
		<JobItem>
			<template #jobTitle>Marketing Planner</template>
		</JobItem>
	</div>
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
