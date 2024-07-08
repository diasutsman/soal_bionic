<template>
	<div id="__BVID__40___BV_modal_content_" tabindex="-1" class="modal-content">
		<header id="__BVID__40___BV_modal_header_" class="modal-header">
			<h5 id="__BVID__40___BV_modal_title_" class="modal-title"></h5>
			<button type="button" aria-label="Close" class="close">×</button>
		</header>
		<div id="__BVID__40___BV_modal_body_" class="modal-body">
			<div class="p-wrh-join-job">
				<div>
					<div>
						<div><p class="pwjj-content-title">Marketing Planner</p></div>
						<div>
							<div class="pwjj-content-description">
								<h5><strong>Job Description :</strong></h5>
								<ul>
									<li>
										Monitor competition to identify new industry trends and
										opportunities for innovation
									</li>
									<li>
										Develop marketing strategies based on customer preferences,
										business objectives, and available resources
									</li>
									<li>
										Conduct market research to identify potential customers and
										assess their needs, interests, and preferences
									</li>
									<li>
										Work with design teams to develop marketing materials such
										as brochures, ads, and presentations
									</li>
									<li>
										Create an advertising budget that reflects the company’s
										priorities while remaining within the parameters set by
										upper management
									</li>
									<li>
										Develop an effective communications strategy for each
										campaign using several different channels, including social
										media, email, push notification, print ads
									</li>
									<li>
										Create a detailed timeline of all marketing activities,
										including production schedules, deadlines for materials
										delivery, and event dates and locations
									</li>
									<li>
										Provide feedback to superiors regarding the effectiveness of
										new campaigns and recommend adjustments
									</li>
								</ul>
								<h5><strong>Skill :</strong></h5>
								<ul>
									<li>Minimum bachelor degree in Marketing Management;</li>
									<li>
										Minimum 3-5 years experience as Marketing Manager/Director
										in any marketplace industry;
									</li>
									<li>Good time management and project management skill;</li>
									<li>
										Creative communication skill in both verbal and design
									</li>
									<li>Multi-language abilities in verbal and non-verbal</li>
								</ul>
							</div>
						</div>
						<div>
							<div class="pwjj-content-title-description pt-4 pb-3">
								Send Your Job Application
							</div>
							<div class="pwjj-content-parent-input">
								<div class="pwjj-content-child-input">
									<label for="YourName" class="pwjj-content-label-input"
										>Your Name</label
									>
									<input
										type="text"
										id="YourName"
										placeholder="Enter your name"
										required="required"
										class="form-control input-outline invalid"
									/>
								</div>
								<div class="pwjj-content-child-input">
									<label for="MobileNumber" class="pwjj-content-label-input"
										>Mobile Number</label
									>
									<input
										type="text"
										id="MobileNumber"
										placeholder="Enter your mobile number"
										required="required"
										class="form-control input-outline invalid"
									/>
								</div>
								<div class="pwjj-content-child-input">
									<label for="EmailAddress" class="pwjj-content-label-input"
										>Email Address</label
									>
									<input
										type="text"
										id="EmailAddress"
										placeholder="Enter your email"
										minlength="5"
										maxlength="254"
										email=""
										required="required"
										class="form-control input-outline invalid"
									/>
									<!---->
								</div>
								<div class="pwjj-content-child-input">
									<label for="WriteMessage" class="pwjj-content-label-input"
										>Write your message here...</label
									>
									<textarea
										type="text"
										form="WriteMessage"
										placeholder="Write your message"
										rows="1"
										required="required"
										maxlength="5000"
										class="form-control input-outline invalid"
										style="resize: none"
									></textarea>
									<!---->
								</div>
								<div class="pwjj-content-child-input">
									<label for="file" class="pwjj-content-label-input"
										>File</label
									>
									<div class="pwjj-content-child-file-image">
										<div class="p-1">
											<button class="pwjj-content-child-file-btn">
												<svg
													aria-hidden="true"
													focusable="false"
													data-prefix="fas"
													data-icon="upload"
													role="img"
													xmlns="http://www.w3.org/2000/svg"
													viewBox="0 0 512 512"
													class="svg-inline--fa fa-upload"
												>
													<path
														fill="currentColor"
														d="M105.4 182.6c12.5 12.49 32.76 12.5 45.25 .001L224 109.3V352c0 17.67 14.33 32 32 32c17.67 0 32-14.33 32-32V109.3l73.38 73.38c12.49 12.49 32.75 12.49 45.25-.001c12.49-12.49 12.49-32.75 0-45.25l-128-128C272.4 3.125 264.2 0 256 0S239.6 3.125 233.4 9.375L105.4 137.4C92.88 149.9 92.88 170.1 105.4 182.6zM480 352h-160c0 35.35-28.65 64-64 64s-64-28.65-64-64H32c-17.67 0-32 14.33-32 32v96c0 17.67 14.33 32 32 32h448c17.67 0 32-14.33 32-32v-96C512 366.3 497.7 352 480 352zM432 456c-13.2 0-24-10.8-24-24c0-13.2 10.8-24 24-24s24 10.8 24 24C456 445.2 445.2 456 432 456z"
														class=""
													></path>
												</svg>
											</button>
										</div>
										<div>
											<input
												hidden="hidden"
												type="file"
												id="file_photo"
												data-cy="att"
												multiple="multiple"
												accept="image/*,.pdf,.doc,.docx"
											/>
										</div>
									</div>
								</div>
							</div>
							<div class="pt-3">
								<button
									type="submit"
									id="save-entity"
									disabled="disabled"
									class="btn btn-sm pwjj-content-btn"
								>
									Send Message
								</button>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
		<!---->
	</div>
</template>
