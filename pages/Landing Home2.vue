<template>
	<div class="relative">
		<!-- Navbar Dropdown 1 row -->
		<nav
			class="font-inter mx-auto h-auto w-full lg:sticky top-0 z-20 bg-[#000]"
			x-data="{isOpen: false, menuOne:false, menuHome:false }"
		>
			<!-- CONTAINER -->
			<div
				class="flex flex-col px-6 py-6 lg:flex-row lg:items-center lg:justify-between lg:px-10 lg:py-4 xl:px-20"
			>
				<!-- SVG LOGO - YOU CAN REPLACE THIS -->
				<a href="https://tailwind-css-template-neo.vercel.app/Landing%20Home">
					<img
						src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f66cdeeb4ddfdae25a26c_%5BA%5D--Navbar%20Brand.png"
						alt=""
						class="inline-block max-h-6"
					/>
				</a>
				<!-- MENU CONTENT 1 -->
				<div
					class="mt-14 flex flex-col space-y-8 lg:mt-0 lg:flex lg:flex-row lg:space-x-1 lg:space-y-0"
					x-bind:class="isOpen ? 'show' : 'hidden'"
				>
					<!--MenuHome -->
					<div class="relative flex flex-col">
						<a
							x-on:click.prevent="menuHome = !menuHome"
							href="#"
							class="text-white flex flex-row rounded-lg hover:text-[#c9fd02] lg:px-6 lg:py-4"
							x-bind:class="menuHome ? 'text-[#c9fd02]' : 'text-white'"
						>
							Home
							<svg
								x-bind:class="menuHome ? 'rotate-180' : 'rotate-0' "
								class="fill-current transition"
								style="width: 24px; height: 24px"
								viewBox="0 0 24 24"
							>
								<path
									d="M7.41,8.58L12,13.17L16.59,8.58L18,10L12,16L6,10L7.41,8.58Z"
								/>
							</svg>
						</a>
						<div
							class="lg:px-75 z-50 flex w-full flex-col rounded-lg bg-[#181818] px-5 py-5 lg:absolute lg:top-20 lg:w-[800px] lg:flex-row lg:flex-wrap lg:py-7 lg:shadow-[0_16px_64px_-15px_rgba(45,96,173,0.15)] xl:w-[950px]"
							x-show="menuHome"
							x-on:click.outside="menuHome = false"
							x-transition:enter="transition ease-out duration-200"
							x-transition:enter-start="opacity-0 translate-y-10"
							x-transition:enter-end="opacity-100 translate-y-0"
							x-transition:leave="transition ease-in duration-200"
							x-transition:leave-start="opacity-100 translate-y-0"
							x-transition:leave-end="opacity-0 translate-y-10"
						>
							<!-- ITEM -->
							<a
								class="flex grow flex-col rounded-lg px-5 py-5 lg:basis-[248px] xl:px-8"
								href="https://tailwind-css-template-neo.vercel.app/Landing%20Home"
							>
								<!-- ICON -->
								<div class="relative">
									<img
										class="w-[40px]"
										src="https://uploads-ssl.webflow.com/64745e0b9655a141ddb0db54/64745e0b9655a141ddb0db35_Ellipse%2030.svg"
										alt=""
									/>
								</div>
								<!-- TEXT -->
								<h2 class="text-white font-inter mb-1 mt-5 text-lg font-medium">
									Landing Home
								</h2>
								<p
									class="font-inter max-w-[250px] text-[14px] leading-[24px] text-[#636262] lg:max-w-[400px]"
								>
									Get a better understanding of where your traffic is coming
									from
								</p>
							</a>
							<!-- ITEM -->
							<a
								class="flex grow flex-col rounded-lg px-5 py-5 lg:basis-[248px] xl:px-8"
								href="https://tailwind-css-template-neo.vercel.app/Landing%20Home2"
							>
								<!-- ICON -->
								<div class="relative">
									<img
										class="w-[40px]"
										src="https://uploads-ssl.webflow.com/64745e0b9655a141ddb0db54/64745e0b9655a141ddb0db35_Ellipse%2030.svg"
										alt=""
									/>
								</div>
								<!-- TEXT -->
								<h2 class="text-white font-inter mb-1 mt-5 text-lg font-medium">
									Landing Home 2
								</h2>
								<p
									class="font-inter max-w-[250px] text-[14px] leading-[24px] text-[#636262] lg:max-w-[400px]"
								>
									Speak directly to your customers in a more meaningful way
								</p>
							</a>
							<!-- ITEM -->
							<a
								class="flex grow flex-col rounded-lg px-5 py-5 lg:basis-[248px] xl:px-8"
								href="https://tailwind-css-template-neo.vercel.app/Landing%20Home3"
							>
								<!-- ICON -->
								<div class="relative">
									<img
										class="w-[40px]"
										src="https://uploads-ssl.webflow.com/64745e0b9655a141ddb0db54/64745e0b9655a141ddb0db35_Ellipse%2030.svg"
										alt=""
									/>
								</div>
								<!-- TEXT -->
								<h2 class="text-white font-inter mb-1 mt-5 text-lg font-medium">
									Landing Home 3
								</h2>
								<p
									class="font-inter max-w-[250px] text-[14px] leading-[24px] text-[#636262] lg:max-w-[400px]"
								>
									Build strategic funnels that will drive your customers to
									convert
								</p>
							</a>
						</div>
					</div>

					<a
						href="https://tailwind-css-template-neo.vercel.app/Landing%20Pricing"
						class="text-white font-inter rounded-lg hover:text-[#c9fd02] lg:px-6 lg:py-4"
						>Pricing</a
					>
					<a
						href="https://tailwind-css-template-neo.vercel.app/Landing%20Blog"
						class="text-white font-inter rounded-lg hover:text-[#c9fd02] lg:px-6 lg:py-4 lg:pb-0"
						>Blog</a
					>

					<a
						href="https://tailwind-css-template-neo.vercel.app/Landing%20About"
						class="text-white font-inter rounded-lg pb-8 lg:pb-0 hover:text-[#c9fd02] lg:px-6 lg:py-4"
						>About</a
					>
				</div>
				<!-- MENU CONTENT 2 -->
				<div
					class="flex flex-col space-y-8 lg:flex lg:flex-row lg:space-x-3 lg:space-y-0"
					x-bind:class="isOpen ? 'show' : 'hidden'"
				>
					<a
						href="https://www.designspark.so/"
						target="_blank"
						class="inline-block rounded-full bg-white px-5 py-3 text-center font-bold text-black transition hover:border-black hover:bg-[#c9fd02]"
						>Get Custom Designs</a
					>
				</div>
				<!-- BURGER MENU -->
				<a
					href="#"
					class="absolute right-5 lg:hidden text-white"
					x-on:click.prevent="isOpen = !isOpen"
				>
					<svg
						width="1.25rem"
						height="1rem"
						viewBox="0 0 20 16"
						fill="none"
						xmlns="http://www.w3.org/2000/svg"
					>
						<path
							d="M19 7H1C0.447715 7 0 7.44772 0 8C0 8.55228 0.447715 9 1 9H19C19.5523 9 20 8.55228 20 8C20 7.44772 19.5523 7 19 7Z"
							fill="currentColor"
						></path>
						<path
							d="M19 0H7C6.44772 0 6 0.447715 6 1C6 1.55228 6.44772 2 7 2H19C19.5523 2 20 1.55228 20 1C20 0.447715 19.5523 0 19 0Z"
							fill="currentColor"
						></path>
						<path
							d="M19 14H11C10.4477 14 10 14.4477 10 15C10 15.5523 10.4477 16 11 16H19C19.5523 16 20 15.5523 20 15C20 14.4477 19.5523 14 19 14Z"
							fill="currentColor"
						></path>
					</svg>
				</a>
			</div>
		</nav>

		<section class="relative">
			<!-- BG Image -->
			<img
				src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28f2_Background%20Image1%20(1).svg"
				alt=""
				class="absolute -z-10 inline-block h-full w-full object-cover"
			/>
			<!-- Container -->
			<div
				class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
			>
				<!-- Component -->
				<div
					class="grid grid-cols-1 items-center gap-8 sm:gap-20 lg:grid-cols-2"
				>
					<!-- Heading Content -->
					<div class="max-w-[720px]">
						<h1 class="mb-3 pb-4 text-4xl font-bold text-white md:text-6xl">
							Fast, Reliable and Secure
						</h1>
						<p class="mb-6 max-w-[528px] text-xl text-[#aeaeae] md:mb-10">
							Lorem ipsum dolor sit amet, consectetur adipiscing elit ut
							aliquam, purus sit amet luctus venenatis, lectus
						</p>
						<div class="flex items-center">
							<a
								href="#"
								class="] mr-5 inline-block rounded-full bg-[#c9fd02] px-6 py-4 text-center font-bold text-black transition hover:border-black hover:bg-white md:mr-6 lg:mr-8"
								>Let's Talk</a
							>
							<a
								href="#"
								class="flex max-w-full flex-row rounded-full border border-solid border-[#636262] px-6 py-4 font-bold"
							>
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28f1_PlayCircle.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p class="text-white">View Showreel</p>
							</a>
						</div>
					</div>
					<!-- Image Div -->
					<div>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28ed_Rectangle%2094.png"
							alt=""
							class="mx-auto inline-block h-full w-full max-w-[640px] rounded-2xl object-cover"
						/>
					</div>
				</div>
			</div>
		</section>

		<section class="bg-black">
			<!-- Container -->
			<div
				class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
				data-aos="fade-up"
				data-aos-duration="900"
			>
				<!-- Component -->
				<div
					class="grid grid-cols-1 items-center gap-8 sm:gap-20 lg:grid-cols-2"
				>
					<!-- Image -->
					<div>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28f4_Rectangle%2094%402x.png"
							alt=""
							class="mx-auto inline-block h-full w-full max-w-[640px] rounded-2xl object-cover"
						/>
					</div>
					<!-- Content -->
					<div>
						<h1 class="mb-6 pb-4 text-4xl font-bold text-white md:text-6xl">
							<span class="text-[#c9fd02]">XYZ</span> Payment App
						</h1>
						<p class="mb-6 max-w-[528px] text-[#aeaeae] md:mb-10 lg:mb-12">
							The XYZ Payment App is a user-friendly mobile application that
							revolutionizes the way you handle your payments and transactions.
							With its intuitive interface and robust functionality, it provides
							a seamless and convenient experience for managing your finances.
						</p>
						<div class="mb-6 flex items-center md:mb-10 lg:mb-12">
							<a href="#" class="flex flex-row font-bold">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28f3_CaretRight.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p class="text-white">Read Full Review</p>
							</a>
						</div>
					</div>
				</div>
			</div>
		</section>

		<section class="bg-[#f7f6f2]">
			<!-- Container -->
			<div
				class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
				data-aos="fade-up"
				data-aos-duration="900"
			>
				<!-- Heading -->
				<div class="mx-auto max-w-3xl text-center">
					<h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">
						Make every step user-centric
					</h2>
					<p
						class="mx-auto mb-8 mt-4 max-w-[528px] text-[#636262] md:mb-12 lg:mb-16"
					>
						Lorem ipsum dolor sit amet consectetur adipiscing elit ut
						aliquam,purus sit amet luctus magna fringilla urna
					</p>
				</div>
				<!-- Features -->
				<div class="grid grid-cols-1 gap-5 sm:grid-cols-2 md:grid-cols-3">
					<!-- Item -->
					<div class="grid grid-cols-1 gap-6 rounded-xl bg-white p-8 md:p-10">
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f66cdeeb4ddfdae25a287_Circle%20Image.svg"
							alt="Features Icon"
							class="inline-block h-16"
						/>
						<p class="text-xl font-semibold">Support</p>
						<p class="text-sm text-[#636262]">
							Lorem ipsum dolor sit amet consectetur adipiscing elit ut aliquam,
							purus sit.
						</p>
					</div>
					<!-- Item -->
					<div class="grid grid-cols-1 gap-6 rounded-xl bg-white p-8 md:p-10">
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f66cdeeb4ddfdae25a285_Circle%20Image-1.svg"
							alt="Features Icon"
							class="inline-block h-16"
						/>
						<p class="text-xl font-semibold">Organise</p>
						<p class="text-sm text-[#636262]">
							Lorem ipsum dolor sit amet consectetur adipiscing elit ut aliquam,
							purus sit.
						</p>
					</div>
					<!-- Item -->
					<div class="grid grid-cols-1 gap-6 rounded-xl bg-white p-8 md:p-10">
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f66cdeeb4ddfdae25a286_Circle%20Image-2.svg"
							alt="Features Icon"
							class="inline-block h-16"
						/>
						<p class="text-xl font-semibold">Flexibility</p>
						<p class="text-sm text-[#636262]">
							Lorem ipsum dolor sit amet consectetur adipiscing elit ut aliquam,
							purus sit.
						</p>
					</div>
				</div>
			</div>
		</section>

		<section>
			<!-- Container -->
			<div
				class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
				data-aos="fade-up"
				data-aos-duration="900"
			>
				<!-- Heading Content -->
				<div class="mx-auto mb-8 max-w-3xl text-center md:mb-12 lg:mb-16">
					<h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">
						What our clients are saying
					</h2>
					<p class="mx-auto mt-4 max-w-[528px] text-[#636262]">
						Lorem ipsum dolor sit amet consectetur adipiscing elit ut
						aliquam,purus sit amet luctus magna fringilla urna
					</p>
				</div>
				<!-- Images -->
				<div class="grid grid-cols-1 gap-8 sm:gap-20 lg:grid-cols-2">
					<img
						src="https://uploads-ssl.webflow.com/6458c625291a94a195e6cf3a/6458c625291a94090ae6cf95_Rectangle%2035.png"
						alt=""
						class="sm:hidden"
					/>
					<div class="hidden h-full w-full grid-cols-5 gap-5 sm:grid">
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28e7_Testimonial%20Standard%20Card.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28e5_Testimonial%20Standard%20Card-18.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28e3_Testimonial%20Standard%20Card-19.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28e1_Testimonial%20Standard%20Card-17.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28d9_Testimonial%20Standard%20Card-15.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28df_Testimonial%20Standard%20Card-14.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28dd_Testimonial%20Standard%20Card-13.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/6458c625291a94a195e6cf3a/6458c625291a94090ae6cf95_Rectangle%2035.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28db_Testimonial%20Standard%20Card-11.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28d7_Testimonial%20Standard%20Card-16.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28d5_Testimonial%20Standard%20Card-10.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28cd_Testimonial%20Standard%20Card-7.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28c5_Testimonial%20Standard%20Card-6.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28cb_Testimonial%20Standard%20Card-2.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28c7_Testimonial%20Standard%20Card-3.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28c9_Testimonial%20Standard%20Card-4.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28d3_Testimonial%20Standard%20Card-1.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28d1_Testimonial%20Standard%20Card-5.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28d3_Testimonial%20Standard%20Card-1.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
						<img
							src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28cf_Testimonial%20Standard%20Card-8.png"
							alt=""
							class="inline-block h-24 w-24 rounded-full object-cover opacity-40"
						/>
					</div>
					<div class="max-[991px]:max-w-[720px]">
						<p class="mb-6 max-w-md text-[#636262] md:mb-10 lg:mb-12">
							Lorem ipsum dolor sit amet, consectetur adipiscing elit ut
							aliquam, purus sit amet luctus venenatis, “Lorem ipsum dolor sit
							amet, consectetur adipiscing elit ut aliquam, purus sit amet
							luctus venenatis, lectus magna fringilla urna, porttitor rhoncus
							dolor purus non enim.
							<br />
							<br />Lorem ipsum dolor sit amet, consectetur adipiscing elit ut
							aliquam, purus sit amet luctus venenatis, lectus magna fringilla
							urna, porttitor rhoncus dolor purus non enim.”
						</p>
						<div class="flex gap-4">
							<img
								src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28e9_Group%2047904.svg"
								alt=""
								class="inline-block h-12"
							/>
							<div>
								<p class="font-bold">John Robert</p>
								<p class="text-sm text-[#636262]">Senior Webflow Developer</p>
							</div>
						</div>
					</div>
				</div>
				<!-- Testimonial -->
				<div class="mx-auto mt-20 flex flex-col items-center">
					<a href="#" class="font-semibold text-black">Check all reviews</a>
				</div>
			</div>
		</section>

		<section class="relative">
			<!-- Background Image -->
			<img
				src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28f9_How%20It%20Works%20BG.svg"
				alt=""
				class="absolute inset-[0%] -z-[1] inline-block h-full w-full object-cover"
			/>
			<!-- Container -->
			<div
				class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
				data-aos="fade-up"
				data-aos-duration="900"
			>
				<!-- Heading Div -->
				<div class="mx-auto mb-8 max-w-3xl text-center md:mb-12 lg:mb-16">
					<p class="text-sm font-bold uppercase text-[#c9fd02]">3 easy steps</p>
					<h2 class="mb-4 mt-6 text-3xl font-extrabold text-white md:text-5xl">
						How it works
					</h2>
					<p class="mx-auto mt-4 max-w-[528px] text-[#aeaeae]">
						Lorem ipsum dolor sit amet consectetur adipiscing elit ut
						aliquam,purus sit amet luctus magna fringilla urna
					</p>
				</div>
				<!-- How it Works -->
				<div class="grid grid-cols-1 gap-5 sm:grid-cols-2 md:grid-cols-3">
					<!-- Item -->
					<div class="grid grid-cols-1 gap-4 rounded-xl bg-[#131313] p-8">
						<div
							class="flex h-12 w-12 flex-col items-center justify-center rounded-full bg-[#c9fd02]"
						>
							<p class="text-xl font-bold">1</p>
						</div>
						<p class="text-xl font-semibold text-white">Find Component</p>
						<p class="text-sm text-[#636262]">
							Lorem ipsum dolor sit amet consectetur adipiscing elit ut aliquam,
							purus sit.
						</p>
					</div>
					<!-- Item -->
					<div class="grid grid-cols-1 gap-4 rounded-xl bg-[#131313] p-8">
						<div
							class="flex h-12 w-12 flex-col items-center justify-center rounded-full bg-[#c9fd02]"
						>
							<p class="text-xl font-bold">2</p>
						</div>
						<p class="text-xl font-semibold text-white">Copy and Paste</p>
						<p class="text-sm text-[#636262]">
							Lorem ipsum dolor sit amet consectetur adipiscing elit ut aliquam,
							purus sit.
						</p>
					</div>
					<!-- Item -->
					<div class="grid grid-cols-1 gap-4 rounded-xl bg-[#131313] p-8">
						<div
							class="flex h-12 w-12 flex-col items-center justify-center rounded-full bg-[#c9fd02]"
						>
							<p class="text-xl font-bold">3</p>
						</div>
						<p class="text-xl font-semibold text-white">Done</p>
						<p class="text-sm text-[#636262]">
							Lorem ipsum dolor sit amet consectetur adipiscing elit ut aliquam,
							purus sit.
						</p>
					</div>
				</div>
			</div>
		</section>

		<section class="relative">
			<!-- BG Image -->
			<img
				src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fa_Get%20Started%20BG.svg"
				alt=""
				class="absolute -z-[1] h-full w-full object-cover"
			/>
			<!-- Container -->
			<div
				class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
				data-aos="fade-up"
				data-aos-duration="900"
			>
				<!-- Component -->
				<div class="flex flex-col items-center">
					<!-- Heading Content -->
					<div class="mb-8 max-w-3xl text-center md:mb-12 lg:mb-16">
						<h2
							class="mb-4 mt-6 text-3xl font-extrabold text-white md:text-5xl"
						>
							Simple &amp; Affordable Pricing
						</h2>
						<div class="mx-auto mt-4 max-w-[528px]">
							<p class="text-[#636262]">
								Simple &amp; fixed pricing. 30 days money-back guarantee
							</p>
						</div>
					</div>
					<!-- Pricing Cards -->
					<div class="grid w-full grid-cols-1 gap-8 md:grid-cols-3 md:gap-4">
						<!-- Pricing Card -->
						<div
							class="mx-auto flex w-full max-w-[416px] flex-col items-start rounded-md bg-[#131313] p-8 text-white"
						>
							<div
								class="mb-4 rounded-lg bg-[#cf8f1329] px-5 py-2 text-[#cf8f13]"
							>
								<p class="font-bold">Basic</p>
							</div>
							<p class="mb-6 font-light text-[#636262] md:mb-10 lg:mb-12">
								Lorem ipsum dolor sit amet consectetur adipiscing elit ut
								aliquam, purus sit
							</p>
							<h2 class="my-6 pb-8 text-3xl font-extrabold md:text-5xl">
								$99<span class="text-sm font-light text-[#636262]">/year</span>
							</h2>
							<a
								href="#"
								class="mb-5 inline-block w-full rounded-lg bg-neutral-900 px-6 py-4 text-center font-bold text-[#636262] transition hover:border-black hover:bg-[#c9fd02] hover:text-black lg:mb-8"
								>Get started</a
							>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Premium Designs</p>
							</div>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Exclusive Freebies</p>
							</div>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Monthly Free Exclusive</p>
							</div>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Customer Support</p>
							</div>
						</div>
						<!-- Pricing Card -->
						<div
							class="mx-auto flex w-full max-w-[416px] flex-col items-start rounded-md bg-[#131313] p-8 text-white"
						>
							<div
								class="mb-4 rounded-lg bg-[#0caeb929] px-5 py-2 text-[#0caeb9]"
							>
								<p class="font-bold">Growth</p>
							</div>
							<p class="mb-6 font-light text-[#636262] md:mb-10 lg:mb-12">
								Lorem ipsum dolor sit amet consectetur adipiscing elit ut
								aliquam, purus sit
							</p>
							<h2 class="my-6 pb-8 text-3xl font-extrabold md:text-5xl">
								$149<span class="text-sm font-light text-[#636262]">/year</span>
							</h2>
							<a
								href="#"
								class="mb-5 inline-block w-full rounded-lg bg-[#c9fd02] px-6 py-4 text-center font-bold text-black transition hover:border-black hover:bg-neutral-900 hover:text-[#636262] md:mb-6 lg:mb-8"
								>Get started</a
							>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Premium Designs</p>
							</div>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Exclusive Freebies</p>
							</div>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Monthly Free Exclusive</p>
							</div>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Customer Support</p>
							</div>
						</div>
						<!-- Pricing Card -->
						<div
							class="mx-auto flex w-full max-w-[416px] flex-col items-start rounded-md bg-[#131313] p-8 text-white"
						>
							<div
								class="mb-4 rounded-lg bg-[#c013cf29] px-5 py-2 text-[#c013cf]"
							>
								<p class="font-bold">Premium</p>
							</div>
							<p class="mb-6 font-light text-[#636262] md:mb-10 lg:mb-12">
								Lorem ipsum dolor sit amet consectetur adipiscing elit ut
								aliquam, purus sit
							</p>
							<h2 class="my-6 pb-8 text-3xl font-extrabold md:text-5xl">
								$249<span class="text-sm font-light text-[#636262]">/year</span>
							</h2>
							<a
								href="#"
								class="mb-5 inline-block w-full rounded-lg bg-neutral-900 px-6 py-4 text-center font-bold text-[#636262] transition hover:border-black hover:bg-[#c9fd02] hover:text-black lg:mb-8"
								>Get started</a
							>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Premium Designs</p>
							</div>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Exclusive Freebies</p>
							</div>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Monthly Free Exclusive</p>
							</div>
							<div class="mt-2 flex flex-row">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fb_akar-icons_circle-check-fill.svg"
									alt=""
									class="mr-2 inline-block w-5"
								/>
								<p>Customer Support</p>
							</div>
						</div>
					</div>
				</div>
			</div>
		</section>

		<section class="relative">
			<!-- Image Background -->
			<img
				src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fd_CTA%20Background%20BG.svg"
				alt=""
				class="absolute inset-[0%] -z-[1] inline-block h-full w-full object-cover"
			/>
			<!-- Container -->
			<div
				class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
				data-aos="fade-up"
				data-aos-duration="900"
			>
				<!-- Component -->
				<div class="mx-auto w-full rounded-[60px] bg-[#101010] px-4">
					<div
						class="mx-auto w-full max-w-3xl py-16 text-center max-[479px]:px-2 md:py-24 lg:py-32"
					>
						<h2 class="mb-8 text-3xl font-extrabold text-white md:text-5xl">
							Fast, Reliable and Secure Payment Platform
						</h2>
						<!-- Features -->
						<div
							class="mx-auto mb-6 flex max-w-[640px] flex-col flex-nowrap items-center justify-center gap-4 sm:flex-row md:mb-10 md:gap-8 lg:mb-12"
						>
							<div class="flex flex-row items-center">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fc_tick-circle.svg"
									alt=""
									class="mr-2 inline-block h-8 w-8"
								/>
								<p class="text-white">300+ UI Blocks</p>
							</div>
							<div class="flex flex-row items-center">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fc_tick-circle.svg"
									alt=""
									class="mr-2 inline-block h-8 w-8"
								/>
								<p class="text-white">Fully responsive</p>
							</div>
							<div class="flex flex-row items-center">
								<img
									src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fc_tick-circle.svg"
									alt=""
									class="mr-2 inline-block h-8 w-8"
								/>
								<p class="text-white">Just copy &amp; paste</p>
							</div>
						</div>
						<a
							href="#"
							class="mb-4 inline-block rounded-full border border-solid border-[#c9fd02] bg-[#c9fd02] px-6 py-4 text-center font-bold text-black transition hover:border-black hover:bg-white"
							>Get Started</a
						>
						<p class="text-[#636262]">No credit card required.</p>
					</div>
				</div>
			</div>
		</section>

		<section class="bg-[#f7f6f2]">
			<!-- Container -->
			<div
				class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
				data-aos="fade-up"
				data-aos-duration="900"
			>
				<!-- Heading -->
				<div class="mx-auto mb-8 max-w-3xl text-center md:mb-12 lg:mb-16">
					<h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">
						Frequently Asked Questions
					</h2>
					<div class="mx-auto mt-4 max-w-[528px]">
						<p class="text-[#636262]">
							Lorem ipsum dolor sit amet consectetur adipiscing elit ut
							aliquam,purus sit amet luctus magna fringilla urna
						</p>
					</div>
				</div>
				<!-- FAQ Items -->
				<div
					class="mb-8 grid gap-4 md:mb-12 lg:mb-16"
					data-aos="fade-up"
					data-aos-duration="900"
				>
					<!-- FAQ Items -->
					<div class="w-full">
						<div
							class="mb-6 w-full rounded-xl bg-white p-8"
							x-data="{ open: false }"
						>
							<div
								class="flex cursor-pointer items-start justify-between"
								x-on:click.prevent="open = !open"
							>
								<div class="text-xl font-bold">
									How this theme is different from others in the market?
								</div>
								<div
									class="relative ml-10 mt-1 flex h-5 w-5 items-center justify-center"
								>
									<div
										class="absolute h-5 w-0.5 bg-[#0b0b1f] transition-transform"
										x-bind:class="open ? 'transform rotate-90' : ''"
									></div>
									<div class="h-0.5 w-5 bg-[#0b0b1f]"></div>
								</div>
							</div>
							<div
								class="w-full max-w-[640px] pt-4 lg:max-w-[960px]"
								x-show="open"
								x-transition:enter="transition ease-out duration-300"
								x-transition:enter-start="transform translate-y--10 opacity-0"
								x-transition:enter-end="transform translate-y-0 opacity-100"
								x-transition:leave="transition ease-in duration-300"
								x-transition:leave-start="transform translate-y-0 opacity-100"
								x-transition:leave-end="transform translate-y--10 opacity-0"
							>
								<p class="tracking-[0.2px]">
									Pellentesque in nisi aliquet, pellentesque purus eget,
									imperdiet turpis. Fusce at enim quis neque viverra convallis.
									Vivamus ut elementum leo, eget tempus nisl. Sed viverra enim
									ac turpis posuere consectetur. Sed enim nibh, consequat vitae
									lacus eu, ullamcorper ullamcorper massa. Pellentesque purus
									eget, imperdiet turpis.
								</p>
							</div>
						</div>
					</div>
					<div class="w-full">
						<div
							class="mb-6 w-full rounded-xl bg-white p-8"
							x-data="{ open: false }"
						>
							<div
								class="flex cursor-pointer items-start justify-between"
								x-on:click.prevent="open = !open"
							>
								<div class="text-xl font-bold">
									What is your policy on distributon
								</div>
								<div
									class="relative ml-10 mt-1 flex h-5 w-5 items-center justify-center"
								>
									<div
										class="absolute h-5 w-0.5 bg-[#0b0b1f] transition-transform"
										x-bind:class="open ? 'transform rotate-90' : ''"
									></div>
									<div class="h-0.5 w-5 bg-[#0b0b1f]"></div>
								</div>
							</div>
							<div
								class="w-full max-w-[640px] pt-4 lg:max-w-[960px]"
								x-show="open"
								x-transition:enter="transition ease-out duration-300"
								x-transition:enter-start="transform translate-y--10 opacity-0"
								x-transition:enter-end="transform translate-y-0 opacity-100"
								x-transition:leave="transition ease-in duration-300"
								x-transition:leave-start="transform translate-y-0 opacity-100"
								x-transition:leave-end="transform translate-y--10 opacity-0"
							>
								<p class="tracking-[0.2px]">
									Pellentesque in nisi aliquet, pellentesque purus eget,
									imperdiet turpis. Fusce at enim quis neque viverra convallis.
									Vivamus ut elementum leo, eget tempus nisl. Sed viverra enim
									ac turpis posuere consectetur. Sed enim nibh, consequat vitae
									lacus eu, ullamcorper ullamcorper massa. Pellentesque purus
									eget, imperdiet turpis.
								</p>
							</div>
						</div>
					</div>
					<div class="w-full">
						<div
							class="mb-6 w-full rounded-xl bg-white p-8"
							x-data="{ open: false }"
						>
							<div
								class="flex cursor-pointer items-start justify-between"
								x-on:click.prevent="open = !open"
							>
								<div class="text-xl font-bold">
									How can I contribute to Flowspark?
								</div>
								<div
									class="relative ml-10 mt-1 flex h-5 w-5 items-center justify-center"
								>
									<div
										class="absolute h-5 w-0.5 bg-[#0b0b1f] transition-transform"
										x-bind:class="open ? 'transform rotate-90' : ''"
									></div>
									<div class="h-0.5 w-5 bg-[#0b0b1f]"></div>
								</div>
							</div>
							<div
								class="w-full max-w-[640px] pt-4 lg:max-w-[960px]"
								x-show="open"
								x-transition:enter="transition ease-out duration-300"
								x-transition:enter-start="transform translate-y--10 opacity-0"
								x-transition:enter-end="transform translate-y-0 opacity-100"
								x-transition:leave="transition ease-in duration-300"
								x-transition:leave-start="transform translate-y-0 opacity-100"
								x-transition:leave-end="transform translate-y--10 opacity-0"
							>
								<p class="tracking-[0.2px]">
									Pellentesque in nisi aliquet, pellentesque purus eget,
									imperdiet turpis. Fusce at enim quis neque viverra convallis.
									Vivamus ut elementum leo, eget tempus nisl. Sed viverra enim
									ac turpis posuere consectetur. Sed enim nibh, consequat vitae
									lacus eu, ullamcorper ullamcorper massa. Pellentesque purus
									eget, imperdiet turpis.
								</p>
							</div>
						</div>
					</div>
					<div class="w-full">
						<div
							class="mb-6 w-full rounded-xl bg-white p-8"
							x-data="{ open: false }"
						>
							<div
								class="flex cursor-pointer items-start justify-between"
								x-on:click.prevent="open = !open"
							>
								<div class="text-xl font-bold">
									How this theme is different from others in the market?
								</div>
								<div
									class="relative ml-10 mt-1 flex h-5 w-5 items-center justify-center"
								>
									<div
										class="absolute h-5 w-0.5 bg-[#0b0b1f] transition-transform"
										x-bind:class="open ? 'transform rotate-90' : ''"
									></div>
									<div class="h-0.5 w-5 bg-[#0b0b1f]"></div>
								</div>
							</div>
							<div
								class="w-full max-w-[640px] pt-4 lg:max-w-[960px]"
								x-show="open"
								x-transition:enter="transition ease-out duration-300"
								x-transition:enter-start="transform translate-y--10 opacity-0"
								x-transition:enter-end="transform translate-y-0 opacity-100"
								x-transition:leave="transition ease-in duration-300"
								x-transition:leave-start="transform translate-y-0 opacity-100"
								x-transition:leave-end="transform translate-y--10 opacity-0"
							>
								<p class="tracking-[0.2px]">
									Pellentesque in nisi aliquet, pellentesque purus eget,
									imperdiet turpis. Fusce at enim quis neque viverra convallis.
									Vivamus ut elementum leo, eget tempus nisl. Sed viverra enim
									ac turpis posuere consectetur. Sed enim nibh, consequat vitae
									lacus eu, ullamcorper ullamcorper massa. Pellentesque purus
									eget, imperdiet turpis.
								</p>
							</div>
						</div>
					</div>
					<!-- Add similar blocks for other questions as needed -->
				</div>
				<div class="mb-8 md:mb-12 lg:mb-16"></div>
				<p class="text-center">
					Can’t find the answer you’re looking for? Reach out to our
					<a href="#" class="text-black">customer support team</a>.
				</p>
			</div>
		</section>

		<footer class="block bg-black">
			<!-- Container -->
			<div
				class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
			>
				<!-- Footer Content -->
				<div class="flex flex-col justify-between md:flex-row">
					<h2
						class="mb-4 w-full max-w-[560px] text-3xl font-extrabold text-white md:text-5xl"
					>
						<span class="text-[#c9fd02]">Lightning fast</span> Webflow Dev made
						easy
					</h2>
					<div class="mt-8 flex-none md:mt-0">
						<div class="mb-4 flex max-w-[272px] items-start">
							<img
								src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fe_MapPin.svg"
								alt=""
								class="mr-3 inline-block"
							/>
							<p class="text-white">
								8502 Preston Rd. Inglewood, Maine 98380, USA
							</p>
						</div>
						<div class="mb-4 flex max-w-[272px] items-start">
							<img
								src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28ff_sms.svg"
								alt=""
								class="mr-3 inline-block"
							/>
							<p class="text-white">support@flowspark.co</p>
						</div>
					</div>
				</div>
				<!-- Divider -->
				<div
					class="mb-20 mt-20 w-full border-[0.5px] border-solid border-[#101010]"
				></div>
				<!-- Footer Footnotes -->
				<div class="flex flex-col items-center justify-between md:flex-row">
					<div class="mb-4 text-center font-semibold sm:text-center md:mb-0">
						<a
							href="#"
							class="inline-block py-1.5 pr-6 text-[#636262] transition hover:text-white sm:py-2 sm:pr-6 lg:pr-12"
							>About</a
						>
						<a
							href="#"
							class="inline-block py-1.5 pr-6 text-[#636262] transition hover:text-white sm:py-2 sm:pr-6 lg:pr-12"
							>Features</a
						>
						<a
							href="#"
							class="inline-block py-1.5 pr-6 text-[#636262] transition hover:text-white sm:py-2 sm:pr-6 lg:pr-12"
							>Works</a
						>
						<a
							href="#"
							class="inline-block py-1.5 pr-6 text-[#636262] transition hover:text-white sm:py-2 sm:pr-6 lg:pr-12"
							>Support</a
						>
						<a
							href="#"
							class="inline-block py-1.5 pr-6 text-[#636262] transition hover:text-white sm:py-2 sm:pr-6 lg:pr-12"
							>Help</a
						>
					</div>
					<p class="text-[#636262]">© Copyright 2021. All rights reserved.</p>
				</div>
			</div>
		</footer>
	</div>
</template>

<script>
	import AOS from "aos";
	import "aos/dist/aos.css";

	export default {
		mounted() {
			AOS.init({
				once: true,
			});
		},
	};
</script>

<style></style>
