<template>
	<div class="main-wrapper">
		<!-- eslint-disable no-mixed-spaces-and-tabs -->
		<section class="cta-section about-me-section p-3 p-lg-5 theme-bgs">
			<div class="container">
				<div class="profile-teaser media flex-column flex-lg-row">
					<div class="media-body">
						<!-- <typewriter ref="typewriter" class="type" :interval="20" :style="{visibility: 'visible'}"> -->
						<h2 class="name font-weight-bold mb-1">
							{{ $t('owner') }}
						</h2>
						<div class="tagline mb-3">
							{{ $t('about.tagline') }}
						</div>
						<i18n
							tag="div"
							path="about.description.all"
							class="bio mb-4"
						>
							<template v-slot:projects>
								<router-link
									class="link"
									img
									exact
									:to="{ name: 'projects' }"
									>{{
										$t('about.description.projects')
									}}</router-link
								>
							</template>
							<template v-slot:resume>
								<router-link
									class="link"
									exact
									:to="{ name: 'resume' }"
									>{{
										$t('about.description.resume')
									}}</router-link
								>
							</template>
						</i18n>

						<!--//bio-->
						<!-- </typewriter> -->
						<div class="mb-4">
							<router-link
								exact
								tag="a"
								:to="{ name: 'projects' }"
								class="btn prj mr-2 mt-2 mb-3"
								><svg
									class="
										svg-inline--fa
										fa-arrow-alt-circle-right fa-w-16
										mr-2
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fas"
									data-icon="arrow-alt-circle-right"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 512 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M256 8c137 0 248 111 248 248S393 504 256 504 8 393 8 256 119 8 256 8zM140 300h116v70.9c0 10.7 13 16.1 20.5 8.5l114.3-114.9c4.7-4.7 4.7-12.2 0-16.9l-114.3-115c-7.6-7.6-20.5-2.2-20.5 8.5V212H140c-6.6 0-12 5.4-12 12v64c0 6.6 5.4 12 12 12z"
									></path></svg
								><!-- <i class="fas fa-arrow-alt-circle-right mr-2"></i> Font Awesome fontawesome.com --><span
									class="d-none d-md-inline"
									>{{ $t('regulars.view') }}</span
								>
								{{ $t('header.links.projects') }}</router-link
							>
							<router-link
								exact
								tag="a"
								:to="{ name: 'resume' }"
								class="btn mt-2 btn-secondary-custom mb-3"
								><svg
									class="
										svg-inline--fa
										fa-file-alt fa-w-12
										mr-2
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fas"
									data-icon="file-alt"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 384 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M224 136V0H24C10.7 0 0 10.7 0 24v464c0 13.3 10.7 24 24 24h336c13.3 0 24-10.7 24-24V160H248c-13.2 0-24-10.8-24-24zm64 236c0 6.6-5.4 12-12 12H108c-6.6 0-12-5.4-12-12v-8c0-6.6 5.4-12 12-12h168c6.6 0 12 5.4 12 12v8zm0-64c0 6.6-5.4 12-12 12H108c-6.6 0-12-5.4-12-12v-8c0-6.6 5.4-12 12-12h168c6.6 0 12 5.4 12 12v8zm0-72v8c0 6.6-5.4 12-12 12H108c-6.6 0-12-5.4-12-12v-8c0-6.6 5.4-12 12-12h168c6.6 0 12 5.4 12 12zm96-114.1v6.1H256V0h6.1c6.4 0 12.5 2.5 17 7l97.9 98c4.5 4.5 7 10.6 7 16.9z"
									></path></svg
								><!-- <i class="fas fa-file-alt mr-2"></i> Font Awesome fontawesome.com --><span
									class="d-none d-md-inline"
									>{{ $t('regulars.view') }}</span
								>
								{{ $t('header.links.resume') }}</router-link
							>
						</div>
					</div>
					<!--//media-body-->
					<div
						ref="img-wrapper"
						class="
							wrapper-img
							profile-image
							position-relative
							ml-lg-5
							mb-3 mb-lg-0
							mr-md-0
						"
					>
						<!-- <v-lazy-image
							class="profile-image"
							:src="require('@/assets/img/SelfPhoto/photo2.jpg')"
							src-placeholder=""
						/>
						<div class="filter"></div> -->
					</div>
				</div>
			</div>
		</section>
		<!--//about-me-section-->

		<section class="overview-section p-3 p-lg-5">
			<div class="container">
				<h2 class="section-title font-weight-bold mb-3 observable">
					{{ $t('about.sections.wid.title') }}
				</h2>
				<div class="section-intro mb-5 observable">
					{{ $t('about.sections.wid.tagline') }}
				</div>
				<div class="row">
					<div class="item observable">
						<div class="item-inner">
							<div class="item-icon">
								<svg
									class="
										svg-inline--fa
										js
										fa-js-square fa-w-14
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fab"
									data-icon="js-square"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 448 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M400 32H48C21.5 32 0 53.5 0 80v352c0 26.5 21.5 48 48 48h352c26.5 0 48-21.5 48-48V80c0-26.5-21.5-48-48-48zM243.8 381.4c0 43.6-25.6 63.5-62.9 63.5-33.7 0-53.2-17.4-63.2-38.5l34.3-20.7c6.6 11.7 12.6 21.6 27.1 21.6 13.8 0 22.6-5.4 22.6-26.5V237.7h42.1v143.7zm99.6 63.5c-39.1 0-64.4-18.6-76.7-43l34.3-19.8c9 14.7 20.8 25.6 41.5 25.6 17.4 0 28.6-8.7 28.6-20.8 0-14.4-11.4-19.5-30.7-28l-10.5-4.5c-30.4-12.9-50.5-29.2-50.5-63.5 0-31.6 24.1-55.6 61.6-55.6 26.8 0 46 9.3 59.8 33.7L368 290c-7.2-12.9-15-18-27.1-18-12.3 0-20.1 7.8-20.1 18 0 12.6 7.8 17.7 25.9 25.6l10.5 4.5c35.8 15.3 55.9 31 55.9 66.2 0 37.8-29.8 58.6-69.7 58.6z"
									></path></svg
								><!-- <i class="fab fa-js-square"></i> Font Awesome fontawesome.com -->
							</div>
							<h3 class="item-title">Vanilla JavaScript</h3>
							<div class="item-desc">
								{{ $t('about.skillset.js') }}
							</div>
						</div>
						<!--//item-inner-->
					</div>
					<!--//item-->
					<div class="item observable">
						<div class="item-inner">
							<div class="item-icon">
								<svg
									class="
										svg-inline--fa
										fa-vuejs
										vue
										fa-w-14
										mr-2
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fab"
									data-icon="vuejs"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 448 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M356.9 64.3H280l-56 88.6-48-88.6H0L224 448 448 64.3h-91.1zm-301.2 32h53.8L224 294.5 338.4 96.3h53.8L224 384.5 55.7 96.3z"
									></path></svg
								><!-- <i class="fab fa-vuejs"></i> Font Awesome fontawesome.com -->
								<svg
									class="
										svg-inline--fa
										fa-react
										react
										fa-w-16
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fab"
									data-icon="react"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 512 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M418.2 177.2c-5.4-1.8-10.8-3.5-16.2-5.1.9-3.7 1.7-7.4 2.5-11.1 12.3-59.6 4.2-107.5-23.1-123.3-26.3-15.1-69.2.6-112.6 38.4-4.3 3.7-8.5 7.6-12.5 11.5-2.7-2.6-5.5-5.2-8.3-7.7-45.5-40.4-91.1-57.4-118.4-41.5-26.2 15.2-34 60.3-23 116.7 1.1 5.6 2.3 11.1 3.7 16.7-6.4 1.8-12.7 3.8-18.6 5.9C38.3 196.2 0 225.4 0 255.6c0 31.2 40.8 62.5 96.3 81.5 4.5 1.5 9 3 13.6 4.3-1.5 6-2.8 11.9-4 18-10.5 55.5-2.3 99.5 23.9 114.6 27 15.6 72.4-.4 116.6-39.1 3.5-3.1 7-6.3 10.5-9.7 4.4 4.3 9 8.4 13.6 12.4 42.8 36.8 85.1 51.7 111.2 36.6 27-15.6 35.8-62.9 24.4-120.5-.9-4.4-1.9-8.9-3-13.5 3.2-.9 6.3-1.9 9.4-2.9 57.7-19.1 99.5-50 99.5-81.7 0-30.3-39.4-59.7-93.8-78.4zM282.9 92.3c37.2-32.4 71.9-45.1 87.7-36 16.9 9.7 23.4 48.9 12.8 100.4-.7 3.4-1.4 6.7-2.3 10-22.2-5-44.7-8.6-67.3-10.6-13-18.6-27.2-36.4-42.6-53.1 3.9-3.7 7.7-7.2 11.7-10.7zM167.2 307.5c5.1 8.7 10.3 17.4 15.8 25.9-15.6-1.7-31.1-4.2-46.4-7.5 4.4-14.4 9.9-29.3 16.3-44.5 4.6 8.8 9.3 17.5 14.3 26.1zm-30.3-120.3c14.4-3.2 29.7-5.8 45.6-7.8-5.3 8.3-10.5 16.8-15.4 25.4-4.9 8.5-9.7 17.2-14.2 26-6.3-14.9-11.6-29.5-16-43.6zm27.4 68.9c6.6-13.8 13.8-27.3 21.4-40.6s15.8-26.2 24.4-38.9c15-1.1 30.3-1.7 45.9-1.7s31 .6 45.9 1.7c8.5 12.6 16.6 25.5 24.3 38.7s14.9 26.7 21.7 40.4c-6.7 13.8-13.9 27.4-21.6 40.8-7.6 13.3-15.7 26.2-24.2 39-14.9 1.1-30.4 1.6-46.1 1.6s-30.9-.5-45.6-1.4c-8.7-12.7-16.9-25.7-24.6-39s-14.8-26.8-21.5-40.6zm180.6 51.2c5.1-8.8 9.9-17.7 14.6-26.7 6.4 14.5 12 29.2 16.9 44.3-15.5 3.5-31.2 6.2-47 8 5.4-8.4 10.5-17 15.5-25.6zm14.4-76.5c-4.7-8.8-9.5-17.6-14.5-26.2-4.9-8.5-10-16.9-15.3-25.2 16.1 2 31.5 4.7 45.9 8-4.6 14.8-10 29.2-16.1 43.4zM256.2 118.3c10.5 11.4 20.4 23.4 29.6 35.8-19.8-.9-39.7-.9-59.5 0 9.8-12.9 19.9-24.9 29.9-35.8zM140.2 57c16.8-9.8 54.1 4.2 93.4 39 2.5 2.2 5 4.6 7.6 7-15.5 16.7-29.8 34.5-42.9 53.1-22.6 2-45 5.5-67.2 10.4-1.3-5.1-2.4-10.3-3.5-15.5-9.4-48.4-3.2-84.9 12.6-94zm-24.5 263.6c-4.2-1.2-8.3-2.5-12.4-3.9-21.3-6.7-45.5-17.3-63-31.2-10.1-7-16.9-17.8-18.8-29.9 0-18.3 31.6-41.7 77.2-57.6 5.7-2 11.5-3.8 17.3-5.5 6.8 21.7 15 43 24.5 63.6-9.6 20.9-17.9 42.5-24.8 64.5zm116.6 98c-16.5 15.1-35.6 27.1-56.4 35.3-11.1 5.3-23.9 5.8-35.3 1.3-15.9-9.2-22.5-44.5-13.5-92 1.1-5.6 2.3-11.2 3.7-16.7 22.4 4.8 45 8.1 67.9 9.8 13.2 18.7 27.7 36.6 43.2 53.4-3.2 3.1-6.4 6.1-9.6 8.9zm24.5-24.3c-10.2-11-20.4-23.2-30.3-36.3 9.6.4 19.5.6 29.5.6 10.3 0 20.4-.2 30.4-.7-9.2 12.7-19.1 24.8-29.6 36.4zm130.7 30c-.9 12.2-6.9 23.6-16.5 31.3-15.9 9.2-49.8-2.8-86.4-34.2-4.2-3.6-8.4-7.5-12.7-11.5 15.3-16.9 29.4-34.8 42.2-53.6 22.9-1.9 45.7-5.4 68.2-10.5 1 4.1 1.9 8.2 2.7 12.2 4.9 21.6 5.7 44.1 2.5 66.3zm18.2-107.5c-2.8.9-5.6 1.8-8.5 2.6-7-21.8-15.6-43.1-25.5-63.8 9.6-20.4 17.7-41.4 24.5-62.9 5.2 1.5 10.2 3.1 15 4.7 46.6 16 79.3 39.8 79.3 58 0 19.6-34.9 44.9-84.8 61.4zm-149.7-15c25.3 0 45.8-20.5 45.8-45.8s-20.5-45.8-45.8-45.8c-25.3 0-45.8 20.5-45.8 45.8s20.5 45.8 45.8 45.8z"
									></path>
								</svg>
							</div>
							<h3 class="item-title">Vue &amp; React</h3>
							<div class="item-desc">
								<!-- These two frameworks (React is library) are the
								way of JavaScript developer. Pages are very
								dynamic without even reloading. My most liked is
								Vue. -->
								{{ $t('about.skillset.vue-react') }}
							</div>
						</div>
						<!--//item-inner-->
					</div>
					<!--//item-->

					<div class="item observable">
						<div class="item-inner">
							<div class="item-icon">
								<svg
									class="
										svg-inline--fa
										fa-node-js
										node
										fa-w-14
										mr-2
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fab"
									data-icon="node-js"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 448 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M224 508c-6.7 0-13.5-1.8-19.4-5.2l-61.7-36.5c-9.2-5.2-4.7-7-1.7-8 12.3-4.3 14.8-5.2 27.9-12.7 1.4-.8 3.2-.5 4.6.4l47.4 28.1c1.7 1 4.1 1 5.7 0l184.7-106.6c1.7-1 2.8-3 2.8-5V149.3c0-2.1-1.1-4-2.9-5.1L226.8 37.7c-1.7-1-4-1-5.7 0L36.6 144.3c-1.8 1-2.9 3-2.9 5.1v213.1c0 2 1.1 4 2.9 4.9l50.6 29.2c27.5 13.7 44.3-2.4 44.3-18.7V167.5c0-3 2.4-5.3 5.4-5.3h23.4c2.9 0 5.4 2.3 5.4 5.3V378c0 36.6-20 57.6-54.7 57.6-10.7 0-19.1 0-42.5-11.6l-48.4-27.9C8.1 389.2.7 376.3.7 362.4V149.3c0-13.8 7.4-26.8 19.4-33.7L204.6 9c11.7-6.6 27.2-6.6 38.8 0l184.7 106.7c12 6.9 19.4 19.8 19.4 33.7v213.1c0 13.8-7.4 26.7-19.4 33.7L243.4 502.8c-5.9 3.4-12.6 5.2-19.4 5.2zm149.1-210.1c0-39.9-27-50.5-83.7-58-57.4-7.6-63.2-11.5-63.2-24.9 0-11.1 4.9-25.9 47.4-25.9 37.9 0 51.9 8.2 57.7 33.8.5 2.4 2.7 4.2 5.2 4.2h24c1.5 0 2.9-.6 3.9-1.7s1.5-2.6 1.4-4.1c-3.7-44.1-33-64.6-92.2-64.6-52.7 0-84.1 22.2-84.1 59.5 0 40.4 31.3 51.6 81.8 56.6 60.5 5.9 65.2 14.8 65.2 26.7 0 20.6-16.6 29.4-55.5 29.4-48.9 0-59.6-12.3-63.2-36.6-.4-2.6-2.6-4.5-5.3-4.5h-23.9c-3 0-5.3 2.4-5.3 5.3 0 31.1 16.9 68.2 97.8 68.2 58.4-.1 92-23.2 92-63.4z"
									></path>
								</svg>
								<!-- <i class="fab fa-node-js"></i> Font Awesome fontawesome.com -->
								<svg
									class="express"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 1333.33 773.55"
									shape-rendering="geometricPrecision"
									text-rendering="geometricPrecision"
									image-rendering="optimizeQuality"
									style="fill: var(--pr-stext)"
									fill-rule="evenodd"
									clip-rule="evenodd"
								>
									<path
										d="M1333.33 753.49c-48.5 12.33-78.5.54-105.41-39.87L1036.5 448.79l-27.67-36.67L785.29 714.5c-25.54 36.38-52.33 52.2-100 39.33l286.25-384.25-266.5-347.09c45.83-8.91 77.5-4.38 105.62 36.67l198.54 268.13 200-266.67c25.62-36.38 53.17-50.2 99.17-36.8l-103.33 137-140 182.29c-16.67 20.83-14.38 35.09.96 55.2l267.33 355.18zM.34 363.16l23.41-115.17c63.75-227.92 325-322.63 505.17-181.8 105.29 82.83 131.46 200 126.25 331.25H61.67C52.76 633.69 222.8 776.27 439.58 703.53c76.04-25.54 120.83-85.09 143.25-159.58 11.38-37.33 30.2-43.17 65.29-32.5-17.91 93.17-58.33 171-143.75 219.71-127.62 72.91-309.8 49.33-405.62-52C41.66 620.36 18.08 545.87 7.5 466.2c-1.67-13.17-5-25.71-7.5-38.33.22-21.56.34-43.11.34-64.67v-.04zm62.41-15.83h536.33c-3.5-170.83-109.87-292.17-255.25-293.2-159.58-1.25-274.17 117.2-281.09 293.2h.01z"
										fill-rule="nonzero"
									/>
								</svg>
							</div>
							<!-- <img draggable="false" src="../assets/expressjs.svg" class="express" alt=""> -->

							<h3 class="item-title">Node &amp; Express</h3>
							<div class="item-desc">
								<!-- JavaScript moves from client-side to
								server-side. Seems cool isn't it? Node.js does
								support data saving in the backend. With the
								help of Express.js we could make MVC pattern or
								modern API's in easy way. -->
								{{ $t('about.skillset.node-express') }}
							</div>
						</div>
						<!--//item-inner-->
					</div>
					<!--//item-->

					<div class="item observable">
						<div class="item-inner">
							<div class="item-icon">
								<svg
									class="
										svg-inline--fa
										fa-python
										python
										fa-w-14
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fab"
									data-icon="python"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 448 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M439.8 200.5c-7.7-30.9-22.3-54.2-53.4-54.2h-40.1v47.4c0 36.8-31.2 67.8-66.8 67.8H172.7c-29.2 0-53.4 25-53.4 54.3v101.8c0 29 25.2 46 53.4 54.3 33.8 9.9 66.3 11.7 106.8 0 26.9-7.8 53.4-23.5 53.4-54.3v-40.7H226.2v-13.6h160.2c31.1 0 42.6-21.7 53.4-54.2 11.2-33.5 10.7-65.7 0-108.6zM286.2 404c11.1 0 20.1 9.1 20.1 20.3 0 11.3-9 20.4-20.1 20.4-11 0-20.1-9.2-20.1-20.4.1-11.3 9.1-20.3 20.1-20.3zM167.8 248.1h106.8c29.7 0 53.4-24.5 53.4-54.3V91.9c0-29-24.4-50.7-53.4-55.6-35.8-5.9-74.7-5.6-106.8.1-45.2 8-53.4 24.7-53.4 55.6v40.7h106.9v13.6h-147c-31.1 0-58.3 18.7-66.8 54.2-9.8 40.7-10.2 66.1 0 108.6 7.6 31.6 25.7 54.2 56.8 54.2H101v-48.8c0-35.3 30.5-66.4 66.8-66.4zm-6.7-142.6c-11.1 0-20.1-9.1-20.1-20.3.1-11.3 9-20.4 20.1-20.4 11 0 20.1 9.2 20.1 20.4s-9 20.3-20.1 20.3z"
									></path></svg
								><!-- <i class="fab fa-python"></i> Font Awesome fontawesome.com -->
								<svg
									class="ml-2"
									xmlns="http://www.w3.org/2000/svg"
									xmlns:xlink="http://www.w3.org/1999/xlink"
									aria-hidden="true"
									focusable="false"
									width="0.79em"
									height="1em"
									style="
										-ms-transform: rotate(360deg);
										-webkit-transform: rotate(360deg);
										transform: rotate(360deg);
									"
									preserveAspectRatio="xMidYMid meet"
									viewBox="0 0 256 326"
								>
									<g fill="#2BA977">
										<path
											d="M114.784 0h53.278v244.191c-27.29 5.162-47.38 7.193-69.117 7.193C33.873 251.316 0 222.245 0 166.412c0-53.795 35.93-88.708 91.608-88.708c8.64 0 15.222.68 23.176 2.717V0zm1.867 124.427c-6.24-2.038-11.382-2.717-17.965-2.717c-26.947 0-42.512 16.437-42.512 45.243c0 28.046 14.88 43.532 42.17 43.532c5.896 0 10.696-.332 18.307-1.351v-84.707z"
										/>
										<path
											d="M255.187 84.26v122.263c0 42.105-3.154 62.353-12.411 79.81c-8.64 16.783-20.022 27.366-43.541 39.055l-49.438-23.297c23.519-10.93 34.901-20.588 42.17-35.327c7.61-15.072 10.01-32.529 10.01-78.445V84.261h53.21z"
										/>
										<path
											d="M196.608 0h53.278v54.135h-53.278V0z"
										/>
									</g>
								</svg>
							</div>

							<h3 class="item-title">Python &amp; Django</h3>
							<div class="item-desc">
								<!-- Python the easy, effective programming language
								that is my first learnt language. Mostly I use
								Python for automation. Django is Python's Web
								framework similar to Node.js. -->
								{{ $t('about.skillset.python-django') }}
							</div>
						</div>
						<!--//item-inner-->
					</div>
					<!--//item-->

					<div class="item observable">
						<div class="item-inner">
							<div class="item-icon">
								<svg
									class="
										svg-inline--fa
										fa-npm
										npm
										fa-w-18
										mr-2
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fab"
									data-icon="npm"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 576 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M288 288h-32v-64h32v64zm288-128v192H288v32H160v-32H0V160h576zm-416 32H32v128h64v-96h32v96h32V192zm160 0H192v160h64v-32h64V192zm224 0H352v128h64v-96h32v96h32v-96h32v96h32V192z"
									></path>
								</svg>
								<svg
									class="
										svg-inline--fa
										fa-gulp
										gulp
										fa-w-8
										mr-2
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fab"
									data-icon="gulp"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 256 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M209.8 391.1l-14.1 24.6-4.6 80.2c0 8.9-28.3 16.1-63.1 16.1s-63.1-7.2-63.1-16.1l-5.8-79.4-14.9-25.4c41.2 17.3 126 16.7 165.6 0zm-196-253.3l13.6 125.5c5.9-20 20.8-47 40-55.2 6.3-2.7 12.7-2.7 18.7.9 5.2 3 9.6 9.3 10.1 11.8 1.2 6.5-2 9.1-4.5 9.1-3 0-5.3-4.6-6.8-7.3-4.1-7.3-10.3-7.6-16.9-2.8-6.9 5-12.9 13.4-17.1 20.7-5.1 8.8-9.4 18.5-12 28.2-1.5 5.6-2.9 14.6-.6 19.9 1 2.2 2.5 3.6 4.9 3.6 5 0 12.3-6.6 15.8-10.1 4.5-4.5 10.3-11.5 12.5-16l5.2-15.5c2.6-6.8 9.9-5.6 9.9 0 0 10.2-3.7 13.6-10 34.7-5.8 19.5-7.6 25.8-7.6 25.8-.7 2.8-3.4 7.5-6.3 7.5-1.2 0-2.1-.4-2.6-1.2-1-1.4-.9-5.3-.8-6.3.2-3.2 6.3-22.2 7.3-25.2-2 2.2-4.1 4.4-6.4 6.6-5.4 5.1-14.1 11.8-21.5 11.8-3.4 0-5.6-.9-7.7-2.4l7.6 79.6c2 5 39.2 17.1 88.2 17.1 49.1 0 86.3-12.2 88.2-17.1l10.9-94.6c-5.7 5.2-12.3 11.6-19.6 14.8-5.4 2.3-17.4 3.8-17.4-5.7 0-5.2 9.1-14.8 14.4-21.5 1.4-1.7 4.7-5.9 4.7-8.1 0-2.9-6-2.2-11.7 2.5-3.2 2.7-6.2 6.3-8.7 9.7-4.3 6-6.6 11.2-8.5 15.5-6.2 14.2-4.1 8.6-9.1 22-5 13.3-4.2 11.8-5.2 14-.9 1.9-2.2 3.5-4 4.5-1.9 1-4.5.9-6.1-.3-.9-.6-1.3-1.9-1.3-3.7 0-.9.1-1.8.3-2.7 1.5-6.1 7.8-18.1 15-34.3 1.6-3.7 1-2.6.8-2.3-6.2 6-10.9 8.9-14.4 10.5-5.8 2.6-13 2.6-14.5-4.1-.1-.4-.1-.8-.2-1.2-11.8 9.2-24.3 11.7-20-8.1-4.6 8.2-12.6 14.9-22.4 14.9-4.1 0-7.1-1.4-8.6-5.1-2.3-5.5 1.3-14.9 4.6-23.8 1.7-4.5 4-9.9 7.1-16.2 1.6-3.4 4.2-5.4 7.6-4.5.6.2 1.1.4 1.6.7 2.6 1.8 1.6 4.5.3 7.2-3.8 7.5-7.1 13-9.3 20.8-.9 3.3-2 9 1.5 9 2.4 0 4.7-.8 6.9-2.4 4.6-3.4 8.3-8.5 11.1-13.5 2-3.6 4.4-8.3 5.6-12.3.5-1.7 1.1-3.3 1.8-4.8 1.1-2.5 2.6-5.1 5.2-5.1 1.3 0 2.4.5 3.2 1.5 1.7 2.2 1.3 4.5.4 6.9-2 5.6-4.7 10.6-6.9 16.7-1.3 3.5-2.7 8-2.7 11.7 0 3.4 3.7 2.6 6.8 1.2 2.4-1.1 4.8-2.8 6.8-4.5 1.2-4.9.9-3.8 26.4-68.2 1.3-3.3 3.7-4.7 6.1-4.7 1.2 0 2.2.4 3.2 1.1 1.7 1.3 1.7 4.1 1 6.2-.7 1.9-.6 1.3-4.5 10.5-5.2 12.1-8.6 20.8-13.2 31.9-1.9 4.6-7.7 18.9-8.7 22.3-.6 2.2-1.3 5.8 1 5.8 5.4 0 19.3-13.1 23.1-17 .2-.3.5-.4.9-.6.6-1.9 1.2-3.7 1.7-5.5 1.4-3.8 2.7-8.2 5.3-11.3.8-1 1.7-1.6 2.7-1.6 2.8 0 4.2 1.2 4.2 4 0 1.1-.7 5.1-1.1 6.2 1.4-1.5 2.9-3 4.5-4.5 15-13.9 25.7-6.8 25.7.2 0 7.4-8.9 17.7-13.8 23.4-1.6 1.9-4.9 5.4-5 6.4 0 1.3.9 1.8 2.2 1.8 2 0 6.4-3.5 8-4.7 5-3.9 11.8-9.9 16.6-14.1l14.8-136.8c-30.5 17.1-197.6 17.2-228.3.2zm229.7-8.5c0 21-231.2 21-231.2 0 0-8.8 51.8-15.9 115.6-15.9 9 0 17.8.1 26.3.4l12.6-48.7L228.1.6c1.4-1.4 5.8-.2 9.9 3.5s6.6 7.9 5.3 9.3l-.1.1L185.9 74l-10 40.7c39.9 2.6 67.6 8.1 67.6 14.6zm-69.4 4.6c0-.8-.9-1.5-2.5-2.1l-.2.8c0 1.3-5 2.4-11.1 2.4s-11.1-1.1-11.1-2.4c0-.1 0-.2.1-.3l.2-.7c-1.8.6-3 1.4-3 2.3 0 2.1 6.2 3.7 13.7 3.7 7.7.1 13.9-1.6 13.9-3.7z"
									></path>
								</svg>
							</div>
							<h3 class="item-title">npm &amp; Gulp</h3>
							<div class="item-desc">
								<!-- npm - Node Package Manager. <br />
								Gulp - Node pipeline builder. <br /> -->
								{{ $t('about.skillset.npm-gulp') }}
							</div>
						</div>
						<!--//item-inner-->
					</div>
					<!--//item-->
					<div class="item observable">
						<div class="item-inner">
							<div class="item-icon">
								<svg
									class="
										svg-inline--fa
										fa-html5
										html
										fa-w-12
										mr-2
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fab"
									data-icon="html5"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 384 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M0 32l34.9 395.8L191.5 480l157.6-52.2L384 32H0zm308.2 127.9H124.4l4.1 49.4h175.6l-13.6 148.4-97.9 27v.3h-1.1l-98.7-27.3-6-75.8h47.7L138 320l53.5 14.5 53.7-14.5 6-62.2H84.3L71.5 112.2h241.1l-4.4 47.7z"
									></path></svg
								><!-- <i class="fab fa-html5 mr-2"></i> Font Awesome fontawesome.com --><svg
									class="
										svg-inline--fa
										fa-css3-alt
										css
										fa-w-12
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fab"
									data-icon="css3-alt"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 384 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M0 32l34.9 395.8L192 480l157.1-52.2L384 32H0zm313.1 80l-4.8 47.3L193 208.6l-.3.1h111.5l-12.8 146.6-98.2 28.7-98.8-29.2-6.4-73.9h48.9l3.2 38.3 52.6 13.3 54.7-15.4 3.7-61.6-166.3-.5v-.1l-.2.1-3.6-46.3L193.1 162l6.5-2.7H76.7L70.9 112h242.2z"
									></path></svg
								><!-- <i class="fab fa-css3-alt"></i> Font Awesome fontawesome.com -->
								<svg
									class="
										svg-inline--fa
										fa-sass fa-w-20
										sass
										ml-2
									"
									aria-hidden="true"
									focusable="false"
									data-prefix="fab"
									data-icon="sass"
									role="img"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 640 512"
									data-fa-i2svg=""
								>
									<path
										fill="currentColor"
										d="M301.84 378.92c-.3.6-.6 1.08 0 0zm249.13-87a131.16 131.16 0 0 0-58 13.5c-5.9-11.9-12-22.3-13-30.1-1.2-9.1-2.5-14.5-1.1-25.3s7.7-26.1 7.6-27.2-1.4-6.6-14.3-6.7-24 2.5-25.29 5.9a122.83 122.83 0 0 0-5.3 19.1c-2.3 11.7-25.79 53.5-39.09 75.3-4.4-8.5-8.1-16-8.9-22-1.2-9.1-2.5-14.5-1.1-25.3s7.7-26.1 7.6-27.2-1.4-6.6-14.29-6.7-24 2.5-25.3 5.9-2.7 11.4-5.3 19.1-33.89 77.3-42.08 95.4c-4.2 9.2-7.8 16.6-10.4 21.6-.4.8-.7 1.3-.9 1.7.3-.5.5-1 .5-.8-2.2 4.3-3.5 6.7-3.5 6.7v.1c-1.7 3.2-3.6 6.1-4.5 6.1-.6 0-1.9-8.4.3-19.9 4.7-24.2 15.8-61.8 15.7-63.1-.1-.7 2.1-7.2-7.3-10.7-9.1-3.3-12.4 2.2-13.2 2.2s-1.4 2-1.4 2 10.1-42.4-19.39-42.4c-18.4 0-44 20.2-56.58 38.5-7.9 4.3-25 13.6-43 23.5-6.9 3.8-14 7.7-20.7 11.4-.5-.5-.9-1-1.4-1.5-35.79-38.2-101.87-65.2-99.07-116.5 1-18.7 7.5-67.8 127.07-127.4 98-48.8 176.35-35.4 189.84-5.6 19.4 42.5-41.89 121.6-143.66 133-38.79 4.3-59.18-10.7-64.28-16.3-5.3-5.9-6.1-6.2-8.1-5.1-3.3 1.8-1.2 7 0 10.1 3 7.9 15.5 21.9 36.79 28.9 18.7 6.1 64.18 9.5 119.17-11.8 61.78-23.8 109.87-90.1 95.77-145.6C386.52 18.32 293-.18 204.57 31.22c-52.69 18.7-109.67 48.1-150.66 86.4-48.69 45.6-56.48 85.3-53.28 101.9 11.39 58.9 92.57 97.3 125.06 125.7-1.6.9-3.1 1.7-4.5 2.5-16.29 8.1-78.18 40.5-93.67 74.7-17.5 38.8 2.9 66.6 16.29 70.4 41.79 11.6 84.58-9.3 107.57-43.6s20.2-79.1 9.6-99.5c-.1-.3-.3-.5-.4-.8 4.2-2.5 8.5-5 12.8-7.5 8.29-4.9 16.39-9.4 23.49-13.3-4 10.8-6.9 23.8-8.4 42.6-1.8 22 7.3 50.5 19.1 61.7 5.2 4.9 11.49 5 15.39 5 13.8 0 20-11.4 26.89-25 8.5-16.6 16-35.9 16-35.9s-9.4 52.2 16.3 52.2c9.39 0 18.79-12.1 23-18.3v.1s.2-.4.7-1.2c1-1.5 1.5-2.4 1.5-2.4v-.3c3.8-6.5 12.1-21.4 24.59-46 16.2-31.8 31.69-71.5 31.69-71.5a201.24 201.24 0 0 0 6.2 25.8c2.8 9.5 8.7 19.9 13.4 30-3.8 5.2-6.1 8.2-6.1 8.2a.31.31 0 0 0 .1.2c-3 4-6.4 8.3-9.9 12.5-12.79 15.2-28 32.6-30 37.6-2.4 5.9-1.8 10.3 2.8 13.7 3.4 2.6 9.4 3 15.69 2.5 11.5-.8 19.6-3.6 23.5-5.4a82.2 82.2 0 0 0 20.19-10.6c12.5-9.2 20.1-22.4 19.4-39.8-.4-9.6-3.5-19.2-7.3-28.2 1.1-1.6 2.3-3.3 3.4-5C434.8 301.72 450.1 270 450.1 270a201.24 201.24 0 0 0 6.2 25.8c2.4 8.1 7.09 17 11.39 25.7-18.59 15.1-30.09 32.6-34.09 44.1-7.4 21.3-1.6 30.9 9.3 33.1 4.9 1 11.9-1.3 17.1-3.5a79.46 79.46 0 0 0 21.59-11.1c12.5-9.2 24.59-22.1 23.79-39.6-.3-7.9-2.5-15.8-5.4-23.4 15.7-6.6 36.09-10.2 62.09-7.2 55.68 6.5 66.58 41.3 64.48 55.8s-13.8 22.6-17.7 25-5.1 3.3-4.8 5.1c.5 2.6 2.3 2.5 5.6 1.9 4.6-.8 29.19-11.8 30.29-38.7 1.6-34-31.09-71.4-89-71.1zm-429.18 144.7c-18.39 20.1-44.19 27.7-55.28 21.3C54.61 451 59.31 421.42 82 400c13.8-13 31.59-25 43.39-32.4 2.7-1.6 6.6-4 11.4-6.9.8-.5 1.2-.7 1.2-.7.9-.6 1.9-1.1 2.9-1.7 8.29 30.4.3 57.2-19.1 78.3zm134.36-91.4c-6.4 15.7-19.89 55.7-28.09 53.6-7-1.8-11.3-32.3-1.4-62.3 5-15.1 15.6-33.1 21.9-40.1 10.09-11.3 21.19-14.9 23.79-10.4 3.5 5.9-12.2 49.4-16.2 59.2zm111 53c-2.7 1.4-5.2 2.3-6.4 1.6-.9-.5 1.1-2.4 1.1-2.4s13.9-14.9 19.4-21.7c3.2-4 6.9-8.7 10.89-13.9 0 .5.1 1 .1 1.6-.13 17.9-17.32 30-25.12 34.8zm85.58-19.5c-2-1.4-1.7-6.1 5-20.7 2.6-5.7 8.59-15.3 19-24.5a36.18 36.18 0 0 1 1.9 10.8c-.1 22.5-16.2 30.9-25.89 34.4z"
									></path>
								</svg>
							</div>
							<h3 class="item-title">HTML, CSS &amp; Sass</h3>
							<div class="item-desc">
								{{ $t('about.skillset.html-css-sass') }}
							</div>
						</div>
						<!--//item-inner-->
					</div>
					<!--//item-->
					<div class="item observable">
						<div class="item-inner">
							<div class="item-icon">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									x="0px"
									y="0px"
									width="40"
									height="40"
									viewBox="0 0 48 48"
									class="mb-2"
									style="fill: #000000"
								>
									<path
										fill="#5d4037"
										d="M42,17.3C42,37.8,24,44,24,44S6,37.8,6,17.3c0-2.5,0.2-4.6,0.4-6.3c0.3-2.5,2-4.5,4.4-5.1 C13.9,5,18.8,4,24,4s10.1,1,13.3,1.9c2.4,0.6,4.1,2.7,4.4,5.1C41.8,12.7,42,14.9,42,17.3z"
									></path>
									<path
										fill="#4caf50"
										d="M24,7c4.9,0,9.5,1,12.5,1.8c1.2,0.3,2,1.3,2.2,2.6c0.2,1.9,0.3,3.9,0.3,5.9c0,15.6-11.5,21.9-15,23.4 c-3.5-1.6-15-7.9-15-23.4c0-2,0.1-4,0.3-5.9c0.1-1.3,1-2.3,2.2-2.6C14.5,8,19.1,7,24,7 M24,4c-5.2,0-10.1,1-13.3,1.9 C8.4,6.5,6.6,8.6,6.4,11C6.2,12.7,6,14.9,6,17.3C6,37.8,24,44,24,44s18-6.2,18-26.7c0-2.5-0.2-4.6-0.4-6.3c-0.3-2.5-2-4.5-4.4-5.1 C34.1,5,29.2,4,24,4L24,4z"
									></path>
									<path
										fill="#dcedc8"
										d="M23 28H25V36H23z"
									></path>
									<path
										fill="#4caf50"
										d="M24,10c0,0-6,5-6,13c0,5.2,3.3,8.5,5,10l1-3l1,3c1.7-1.5,5-4.8,5-10C30,15,24,10,24,10z"
									></path>
									<path
										fill="#81c784"
										d="M24,10c0,0-6,5-6,13c0,5.2,3.3,8.5,5,10l1-3V10z"
									></path>
								</svg>
							</div>
							<h3 class="item-title">Mongo DB</h3>
							<div class="item-desc">
								{{ $t('about.skillset.mongo-postgre') }}
							</div>
						</div>
						<!--//item-inner-->
					</div>
					<!--//item-->
				</div>
				<!--//row-->
				<div class="text-center py-3 observable">
					<router-link
						exact
						:to="{ name: 'servicesPricing' }"
						class="btn prj"
						><svg
							class="
								svg-inline--fa
								fa-arrow-alt-circle-right fa-w-16
								mr-2
							"
							aria-hidden="true"
							focusable="false"
							data-prefix="fas"
							data-icon="arrow-alt-circle-right"
							role="img"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 512 512"
							data-fa-i2svg=""
						>
							<path
								fill="currentColor"
								d="M256 8c137 0 248 111 248 248S393 504 256 504 8 393 8 256 119 8 256 8zM140 300h116v70.9c0 10.7 13 16.1 20.5 8.5l114.3-114.9c4.7-4.7 4.7-12.2 0-16.9l-114.3-115c-7.6-7.6-20.5-2.2-20.5 8.5V212H140c-6.6 0-12 5.4-12 12v64c0 6.6 5.4 12 12 12z"
							></path></svg
						>{{ $t('header.links.services') }}
					</router-link>
				</div>
			</div>
			<!--//container-->
		</section>

		<!-- <div class="container"><hr></div> -->

		<!--//testimonials-section-->

		<div class="container"><hr /></div>

		<section class="featured-section p-3 p-lg-5">
			<div class="container">
				<h2 class="section-title font-weight-bold mb-5 observable">
					{{ $t('about.sections.featured') }}
				</h2>
				<transition name="projectLoaded">
					<app-loading
						:condition="featuredProjectsLoading"
					></app-loading>
				</transition>

				<div
					v-show-slide:400:ease="!featuredProjectsLoading"
					class="grid-per-2x2 t3d-section"
				>
					<div
						v-for="(project, index) in featuredProjects"
						:key="project._id"
						:id="index"
						@mouseleave="onMouseLeave($event, index)"
						@mouseenter="onMouseEnter($event, index)"
						@mousemove="onMouseMove($event, index)"
						ref="skillcard"
						class="card-wrapper py-5 px-4"
						style="height: auto !important"
					>
						<div class="observable">
							<div class="card fafa about-card project-card">
								<div class="row no-gutters">
									<div
										class="
											col-lg-4
											card-img-holder
											project-card-img
											tr
											position-relative
										"
									>
										<v-lazy-image
											:src="project.image"
											:src-placeholder="project.title"
										/>
										<div class="filter"></div>
										<!-- <img :src="projects.imgSrc" class="card-img" alt="image"> -->
									</div>
									<div class="col-lg-8 h-100">
										<div class="card-body h-100">
											<h5 class="card-title tr">
												<a
													:href="project.url"
													class="theme-link z"
													>{{ project.title }}</a
												>
											</h5>
											<p class="card-text1 tr">
												{{ project.description }}
											</p>
											<p class="card-text tr">
												<small class="text-muted"
													>Client:
													{{ project.client }}</small
												>
											</p>
										</div>
									</div>
								</div>
								<div class="link-mask tr">
									<div class="link-mask-text">
										<a
											class="
												btn
												watch
												btn-secondary-custom
											"
											:href="project.url"
										>
											<svg
												class="
													svg-inline--fa
													fa-eye fa-w-18
													mr-2
												"
												aria-hidden="true"
												focusable="false"
												data-prefix="fas"
												data-icon="eye"
												role="img"
												xmlns="http://www.w3.org/2000/svg"
												viewBox="0 0 576 512"
												data-fa-i2svg=""
											>
												<path
													fill="currentColor"
													d="M572.52 241.4C518.29 135.59 410.93 64 288 64S57.68 135.64 3.48 241.41a32.35 32.35 0 0 0 0 29.19C57.71 376.41 165.07 448 288 448s230.32-71.64 284.52-177.41a32.35 32.35 0 0 0 0-29.19zM288 400a144 144 0 1 1 144-144 143.93 143.93 0 0 1-144 144zm0-240a95.31 95.31 0 0 0-25.31 3.79 47.85 47.85 0 0 1-66.9 66.9A95.78 95.78 0 1 0 288 160z"
												></path></svg
											><!-- <i class="fas fa-eye mr-2"></i> Font Awesome fontawesome.com -->View
											Case Study
										</a>
									</div>
								</div>
								<!--//link-mask-->
							</div>
							<!--//card-->
						</div>
					</div>
					<!--//col-->
				</div>

				<!--//row-->
				<div class="text-center py-3 observable">
					<router-link
						exact
						:to="{ name: 'projects' }"
						class="btn prj"
						><svg
							class="
								svg-inline--fa
								fa-arrow-alt-circle-right fa-w-16
								mr-2
							"
							aria-hidden="true"
							focusable="false"
							data-prefix="fas"
							data-icon="arrow-alt-circle-right"
							role="img"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 512 512"
							data-fa-i2svg=""
						>
							<path
								fill="currentColor"
								d="M256 8c137 0 248 111 248 248S393 504 256 504 8 393 8 256 119 8 256 8zM140 300h116v70.9c0 10.7 13 16.1 20.5 8.5l114.3-114.9c4.7-4.7 4.7-12.2 0-16.9l-114.3-115c-7.6-7.6-20.5-2.2-20.5 8.5V212H140c-6.6 0-12 5.4-12 12v64c0 6.6 5.4 12 12 12z"
							></path>
						</svg>
						{{ $t('regulars.view') }}
						{{ $t('header.links.projects') }}</router-link
					>
				</div>
			</div>
			<!--//container-->
		</section>
		<!--//featured-section-->

		<div class="container"><hr /></div>

		<section class="latest-blog-section p-3 p-lg-5">
			<div class="container">
				<h2 class="section-title font-weight-bold mb-5 observable">
					{{ $t('about.sections.lbp') }}
				</h2>
				<transition name="projectLoaded">
					<app-loading
						:condition="featuredProjectsLoading"
					></app-loading>
				</transition>
				<div v-if="!featuredProjectsLoading" class="grid-per-3x1 pt-5">
					<div
						class="mx-2 mb-5 observable"
						v-for="(blog, index) in latestBlogs"
						:key="index"
					>
						<div class="card blog-post-card">
							<video
								v-if="blog.posterType === 'video'"
								class="card-img-top"
								preload="metadata"
								paused="true"
							>
								<source :src="blog.poster" type="video/mp4" />
							</video>
							<img
								v-else
								class="card-img-top"
								:src="blog.poster"
								:alt="blog.heading"
							/>
							<div class="card-body">
								<h5 class="card-title">
									<router-link
										:to="{
											name: 'particular-blog',
											params: { slug: blog.slug }
										}"
										>{{ blog.heading }}</router-link
									>
								</h5>
								<p class="card-text">
									{{ blog.tag }}
									<br />
									<br />
									<b class="blog-lang"
										>Language: {{ blog.language }}</b
									>
								</p>
								<p class="mb-0">
									<router-link
										:to="{
											name: 'particular-blog',
											params: { slug: blog.slug }
										}"
										>{{
											$t('regulars.readMore')
										}}
										→</router-link
									>
								</p>
							</div>
							<div class="card-footer">
								<small class="text-muted"
									>{{ $t('regulars.published') }}
									{{ blog.publishedDate }}</small
								>
							</div>
						</div>
						<!--//card-->
					</div>
					<!--//col-->
				</div>
				<!--//row-->
				<div class="text-center py-3 observable">
					<router-link exact :to="{ name: 'blog' }" class="btn prj"
						><svg
							class="
								svg-inline--fa
								fa-arrow-alt-circle-right fa-w-16
								mr-2
							"
							aria-hidden="true"
							focusable="false"
							data-prefix="fas"
							data-icon="arrow-alt-circle-right"
							role="img"
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 512 512"
							data-fa-i2svg=""
						>
							<path
								fill="currentColor"
								d="M256 8c137 0 248 111 248 248S393 504 256 504 8 393 8 256 119 8 256 8zM140 300h116v70.9c0 10.7 13 16.1 20.5 8.5l114.3-114.9c4.7-4.7 4.7-12.2 0-16.9l-114.3-115c-7.6-7.6-20.5-2.2-20.5 8.5V212H140c-6.6 0-12 5.4-12 12v64c0 6.6 5.4 12 12 12z"
							></path></svg
						>{{ $t('regulars.view') }}
						{{ $t('header.links.blog') }}</router-link
					>
				</div>
			</div>
			<!--//container-->
		</section>
		<!--//latest-blog-section-->
	</div>
	<!-- eslint-enable no-mixed-spaces-and-tabs -->
</template>

<script>
import { BrowserDetect } from '@/assets/jsComponents/browserDetect'
import {
	onMouseEnter,
	onMouseLeave,
	onMouseMove
} from '@/assets/jsComponents/3dAnimation.js'

import { mapState, mapActions } from 'vuex'
import hoverEffect from 'hover-effect'

// eslint-disable no-mixed-spaces-and-tabs
export default {
	data() {
		return {
			status: 'hidden',
			browser: BrowserDetect.browser
		}
	},
	computed: {
		...mapState('Blogs', ['latestBlogs']),
		...mapState('Projects', ['featuredProjects']),

		featuredProjectsLoading() {
			return this.featuredProjects.length === 0
		}
	},

	methods: {
		onMouseEnter,
		onMouseLeave,
		onMouseMove,
		onLoad() {
			if (this.latestBlogs.length === 0) {
				this.setLatestBlogs()
			}
			if (this.featuredProjects.length === 0) {
				this.setFeaturedProjects()
			}
		},
		initializeHoverEffect() {
			setTimeout(() => {
				new hoverEffect({
					parent: this.$refs['img-wrapper'],
					image1: require('../assets/img/SelfPhoto/photo2-min.jpg'),
					image2: require('../assets/img/SelfPhoto/photo1-min.jpg'),
					displacementImage: require('../assets/img/ramen.jpg'),
					intensity: 0.05,
					angle: 1 / 12,
					imagesRatio: 256 / 384
				})
			}, 10)
		},

		...mapActions('Projects', ['setFeaturedProjects']),
		...mapActions('Blogs', ['setLatestBlogs'])
	},
	mounted() {
		this.$intersectionAnimation()
		this.initializeHoverEffect()
	},
	created() {
		this.onLoad()
	},
	updated() {
		this.$intersectionAnimation()
	},

	head() {
		return {
			title: this.$t('header.links.about'),
			meta: [
				{
					name: 'description',
					content: this.$t('about.description.all', {
						projects: this.$t('about.description.projects'),
						resume: this.$t('about.description.resume')
					})
				},
				{
					name: 'og:description',
					content: this.$t('about.description.all', {
						projects: this.$t('about.description.projects'),
						resume: this.$t('about.description.resume')
					})
				},
				{
					property: 'og:title',
					content: this.$t('header.links.about')
				}
			]
		}
	}
}
// eslint-enable no-mixed-spaces-and-tabs
</script>

<style lang="scss" scoped>
.main-wrapper {
	-webkit-perspective: 600px;
	-moz-perspective: 600px;
	-ms-perspective: 600px;
	perspective: 600px;
	perspective-origin: 50% 50%;
}
</style>
