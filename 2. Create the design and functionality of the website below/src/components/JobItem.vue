<template>
	<div class="pwrh-child-job">
		<div class="pwrh-content-job">
			<p class="pwrh-content-title">
				<slot name="jobTitle"></slot>
			</p>

			<div>
				<button class="pwrh-content-btn">See Job</button>
			</div>
		</div>
	</div>
</template>

<style scoped>
.pwrh-child-job {
}

.pwrh-child-job .pwrh-content-job {
	-webkit-box-align: center;
	-ms-flex-align: center;
	align-items: center;
	background: #f0ede5;
	border-radius: 10px;
	-webkit-box-shadow: 0 4px 4px rgba(0, 0, 0, 0.25);
	box-shadow: 0 4px 4px rgba(0, 0, 0, 0.25);
	display: -webkit-box;
	display: -ms-flexbox;
	display: flex;
	/* margin-bottom: 1rem;
	margin-left: 1rem;
	margin-right: 1rem; */
	padding: 1rem;

	/* Flex stuff */
	justify-content: space-between;
}

.pwrh-child-job .pwrh-content-job .pwrh-content-title {
	color: #4b9741;
	font-weight: 700;
	margin-left: 1rem;
}

.pwrh-child-job .pwrh-content-job .pwrh-content-btn {
	background: #f09506;
	border: 1px solid #f09506;
	border-radius: 5px;
	color: #fff;
	font-weight: 700;
	padding-left: 1rem;
	padding-right: 1rem;
	white-space: nowrap;
}
</style>
