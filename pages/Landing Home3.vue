<template>
  <div class="overflow-hidden">
      <!-- Navbar Dropdown 1 row -->
    <section>
      <div class="h-auto w-screen bg-black text-white">
        <!-- NAVBAR -->
        <nav
          class="font-inter mx-auto h-auto w-full max-w-[1600px] lg:relative lg:top-0"
          x-data="{isOpen: false, menuOne:false, menuHome:false }"
        >
          <!-- CONTAINER -->
          <div
            class="flex flex-col px-6 py-6 lg:flex-row lg:items-center lg:justify-between lg:px-10 lg:py-4 xl:px-20"
          >
            <!-- SVG LOGO - YOU CAN REPLACE THIS -->
            <a
              href="https://tailwind-css-template-neo.vercel.app/Landing%20Home"
            >
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
              <!-- DROPDOWN -->
              <div class="relative flex flex-col">
                <a
                  x-on:click.prevent="menuOne = !menuOne"
                  href="#"
                  class="flex flex-row rounded-lg hover:text-[#c9fd02] lg:px-6 lg:py-4"
                  x-bind:class="menuOne ? ' text-[#c9fd02] ' : 'text-white  ' "
                  >Component
                  <svg
                    x-bind:class="menuOne ? 'rotate-180' : 'rotate-0' "
                    class="fill-current transition"
                    style="width: 24px; height: 24px"
                    viewBox="0 0 24 24"
                  >
                    <path
                      d="M7.41,8.58L12,13.17L16.59,8.58L18,10L12,16L6,10L7.41,8.58Z"
                    />
                  </svg>
                </a>
                <!-- DROP DOWN MENU ONE -->
                <div
                  class="lg:px-75 z-50 flex w-full flex-col rounded-lg bg-[#181818] px-5 py-5 lg:absolute lg:top-20 lg:w-[800px] lg:flex-row lg:flex-wrap lg:py-7 lg:shadow-[0_16px_64px_-15px_rgba(45,96,173,0.15)] xl:w-[950px]"
                  x-show="menuOne"
                  x-on:click.outside="menuOne = false"
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
                    href="#"
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
                    <h2 class="font-inter mb-1 mt-5 text-lg font-medium">
                      Analytics
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
                    href="#"
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
                    <h2 class="font-inter mb-1 mt-5 text-lg font-medium">
                      Engagement
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
                    href="#"
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
                    <h2 class="font-inter mb-1 mt-5 text-lg font-medium">
                      Automations
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
                href="https://tailspark.co/templates"
                target="_blank"
                class="font-inter rounded-lg hover:text-[#c9fd02] lg:px-6 lg:py-4"
                >Templates</a
              >
              <a
                href="https://tailwind-css-template-neo.vercel.app/Landing%20Pricing"
                class="font-inter rounded-lg hover:text-[#c9fd02] lg:px-6 lg:py-4"
                >Pricing</a
              >
              <a
                href="https://tailwind-css-template-neo.vercel.app/Landing%20Blog"
                class="font-inter rounded-lg hover:text-[#c9fd02] lg:px-6 lg:py-4 lg:pb-0"
                >Blog</a
              >

              <a
                href="https://tailwind-css-template-neo.vercel.app/Landing%20About"
                class="font-inter rounded-lg pb-8 hover:text-[#c9fd02] lg:px-6 lg:py-4 lg:pb-0"
                >About</a
              >
              <!--MenuHome -->
              <div class="relative flex flex-col">
                <a
                  x-on:click.prevent="menuHome = !menuHome"
                  href="#"
                  class="flex flex-row rounded-lg hover:text-[#c9fd02] lg:px-6 lg:py-4"
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
                  class="z-50 flex gap-5 w-full flex-col rounded-lg bg-[#181818] p-5 lg:absolute lg:top-20 lg:w-[200px] lg:flex-wrap lg:shadow-[0_16px_64px_-15px_rgba(45,96,173,0.15)]"
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
                  <a href="https://tailwind-css-template-neo.vercel.app/Landing%20Home">
                    <!-- TEXT -->
                    <h2 class="font-inter text-lg font-medium">Landing Home</h2>
                  </a>
                  <!-- ITEM -->
                  <a
                    href="https://tailwind-css-template-neo.vercel.app/Landing%20Home2"
                  >
                    <!-- TEXT -->
                    <h2 class="font-inter text-lg font-medium">
                      Landing Home 2
                    </h2>
                  </a>
                  <!-- ITEM -->
                  <a
                    href="https://tailwind-css-template-neo.vercel.app/Landing%20Home3"
                  >
                    <!-- TEXT -->
                    <h2 class="font-inter text-lg font-medium">
                      Landing Home 3
                    </h2>
                  </a>
                </div>
              </div>
            </div>
            <!-- MENU CONTENT 2 -->
            <div
              class="flex flex-col space-y-8 lg:flex lg:flex-row lg:space-x-3 lg:space-y-0"
              x-bind:class="isOpen ? 'show' : 'hidden'"
            >
              <a
                href="https://flowspark.co/design"
                target="_blank"
                class="inline-block rounded-full bg-white px-5 py-3 text-center font-bold text-black transition hover:border-black hover:bg-[#c9fd02]"
                >Get Custom Designs</a
              >
            </div>
            <!-- BURGER MENU -->
            <a
              href="#"
              class="absolute right-5 lg:hidden"
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
      </div>
    </section>

    <section>
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
          <!-- Heading Div -->
          <div class="max-w-[720px]">
            <h1 class="mb-6 pb-4 text-4xl font-bold md:text-6xl">
              Fast,Reliable and Secure
            </h1>
            <p class="mb-6 max-w-[528px] text-[#636262] md:mb-10 lg:mb-12">
              Say goodbye to payment headaches with SecurePay! Our easy-to-use
              payment platform makes it simple for businesses and individuals to
              send and receive payments
            </p>
            <a
              href="#"
              class="mb-5 mr-5 inline-block rounded-full bg-[#c9fd02] px-6 py-4 text-center font-bold text-black transition hover:border-black hover:bg-white lg:mb-8 lg:mr-8"
              >Open Account</a
            >
            <div class="w-full max-w-xs">
              <!-- Testimonial -->
              <div
                class="mb-4 py-1.5 pl-4 [border-left:2px_solid_rgb(201,_253,_2)]"
              >
                <p class="text-sm text-[#636262]">
                  A secure and convenient payment app that makes transactions a
                  breeze, offering a seamless way to manage finances on the go.
                </p>
              </div>
              <!-- Author -->
              <div class="flex items-center">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c349_Ellipse%2020%20(1).png"
                  alt=""
                  class="mr-2 inline-block h-7 w-7"
                />
                <p class="text-sm font-bold">Jessica Smith</p>
                <div class="mx-4 h-full py-3 [border-right-style:solid]"></div>
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <p class="text-sm text-[#636262]">5 stars</p>
              </div>
            </div>
          </div>
          <!-- Image Div -->
          <div>
            <img
              src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c34b_Rectangle%2094.svg"
              alt=""
              class="mx-auto inline-block h-full w-full max-w-[640px] rounded-2xl object-cover"
            />
          </div>
        </div>
      </div>
    </section>

    <section class="relative text-white">
      <!-- BG Image -->
      <img
        src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c34c_Pricing%20BG%20(1).svg"
        alt=""
        class="absolute -z-10 inline-block h-full w-full object-cover"
      />
      <!-- Container -->
      <div
        class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
        data-aos="fade-up"
        data-aos-duration="900"
      >
        <!-- Heading Content -->
        <div class="mx-auto mb-8 max-w-3xl text-center md:mb-12 lg:mb-16">
          <h2 class="mb-4 mt-6 text-3xl font-extrabold text-white md:text-5xl">
            Backed up by real data
          </h2>
          <p class="mx-auto mt-4 max-w-[528px] text-[#636262]">
            Lorem ipsum dolor sit amet consectetur adipiscing elit ut
            aliquam,purus sit amet luctus magna fringilla urna
          </p>
        </div>
        <!-- Facts -->
        <div
          class="py- lg:grid-cols-48 mx-auto grid w-full max-w-[960px] grid-cols-1 gap-5 px-16 sm:grid-cols-2 md:grid-cols-3 md:gap-12 lg:grid-cols-4"
        >
          <!-- Fact Item -->
          <div class="flex flex-col items-center gap-4">
            <p>Blocks</p>
            <h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">
              200<span class="text-[#c9fd02]">+</span>
            </h2>
          </div>
          <!-- Fact Item -->
          <div class="flex flex-col items-center gap-4">
            <p>Templates</p>
            <h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">45</h2>
          </div>
          <!-- Fact Item -->
          <div class="flex flex-col items-center gap-4">
            <p>Customers</p>
            <h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">
              1500<span class="text-[#c9fd02]">+</span>
            </h2>
          </div>
          <!-- Fact Item -->
          <div class="flex flex-col items-center gap-4">
            <p>Support Tickets</p>
            <h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">890</h2>
          </div>
          <div class=""></div>
        </div>
      </div>
    </section>

    <section class="relative">
      <!-- BG Image -->
      <img
        src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c34c_Pricing%20BG%20(1).svg"
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
        <div
          class="rounded-[60px] bg-[#101010] px-12 py-16 text-white md:py-24 lg:py-32"
        >
          <!-- Heading Content -->
          <div class="mx-auto mb-8 max-w-3xl text-center md:mb-12 lg:mb-16">
            <h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">
              Simple &amp; Affordable Pricing
            </h2>
            <div class="mx-auto mt-4 max-w-[528px]">
              <p class="text-[#636262]">
                Simple &amp; fixed pricing. 30 days money-back guarantee
              </p>
            </div>
          </div>
          <!-- Pricing Content -->
          <div
            class="mx-auto grid h-auto w-full grid-cols-1 gap-4 rounded-md bg-[#f2f2f700] py-12 lg:grid-cols-2"
          >
            <!-- Pricing Features -->
            <div
              class="grid grid-cols-1 gap-4 rounded-xl border border-solid border-[#181818] px-10 py-14 sm:grid-cols-2"
            >
              <div class="flex flex-row items-center">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fc_tick-circle.svg"
                  alt=""
                  class="mr-4 inline-block h-4 w-4"
                />
                <p>Premium Designs</p>
              </div>
              <div class="flex flex-row items-center">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fc_tick-circle.svg"
                  alt=""
                  class="mr-4 inline-block h-4 w-4"
                />
                <p>Regular updates</p>
              </div>
              <div class="flex flex-row items-center">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fc_tick-circle.svg"
                  alt=""
                  class="mr-4 inline-block h-4 w-4"
                />
                <p>Copy &amp; Paste</p>
              </div>
              <div class="flex flex-row items-center">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fc_tick-circle.svg"
                  alt=""
                  class="mr-4 inline-block h-4 w-4"
                />
                <p>Lifetime Access</p>
              </div>
              <div class="flex flex-row items-center">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fc_tick-circle.svg"
                  alt=""
                  class="mr-4 inline-block h-4 w-4"
                />
                <p>Early bird price</p>
              </div>
              <div class="flex flex-row items-center">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f68133fc5cb4e29ed28fc_tick-circle.svg"
                  alt=""
                  class="mr-4 inline-block h-4 w-4"
                />
                <p>Premium Support</p>
              </div>
            </div>
            <!-- Pricing Cost -->
            <div class="flex flex-col rounded-xl bg-[#181818] p-10">
              <div
                class="flex w-full flex-col items-center justify-between sm:flex-row"
              >
                <h2
                  class="mb-4 mt-6 text-left text-3xl font-extrabold md:text-5xl"
                >
                  $149<span class="text-sm font-light text-[#636262]"
                    >/month</span
                  >
                </h2>
                <a
                  href="#"
                  class="inline-block rounded-[60px] border border-solid border-[#c9fd02] bg-[#c9fd02] px-6 py-4 text-center font-bold text-black transition hover:border-black hover:bg-white"
                  >Get started</a
                >
              </div>
              <!-- Divider -->
              <div
                class="mb-6 mt-6 w-full border-[0.5px] border-solid border-[#242424]"
              ></div>
              <p class="text-sm text-[#636262]">
                Lorem ipsum dolor sit amet consectetur adipiscing elit ut
                aliquam,purus sit amet luctus magna fringilla urna
              </p>
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
        <h2
          class="mx-auto mb-8 mt-6 max-w-3xl text-center text-3xl font-extrabold md:mb-16 md:text-5xl"
        >
          What our clients are saying
        </h2>
        <!-- Testimonails -->
        <div class="mb-5 grid grid-cols-1 gap-5 md:grid-cols-2 lg:mb-8">
          <!-- Item -->
          <div
            class="grid min-h-[280px] grid-cols-[1fr_1.75fr] gap-6 rounded-2xl bg-white p-8 md:p-10"
          >
            <!-- Author -->
            <div class="flex flex-col justify-between">
              <div class="flex flex-col items-start gap-4">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c34e_Image%20%26%20Quotation.svg"
                  alt=""
                  class="inline-block h-16"
                />
                <div class="flex flex-col">
                  <h6 class="text-sm font-bold md:text-base">Jonathan Smith</h6>
                  <p class="text-sm text-[#636262]">Small Business Owner</p>
                </div>
              </div>
              <div class="flex">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
              </div>
            </div>
            <p class="text-[#636262]">
              “Lorem ipsum dolor sit amet, &nbsp;elit ut aliquam, purus sit amet
              luctus venenatis elit ut aliquam, purus sit amet luctus venenatis"
            </p>
          </div>
          <!-- Item -->
          <div
            class="grid min-h-[280px] grid-cols-[1fr_1.75fr] gap-6 rounded-2xl bg-white p-8 md:p-10"
          >
            <!-- Author -->
            <div class="flex flex-col justify-between">
              <div class="flex flex-col items-start gap-4">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c350_Image%20%26%20Quotation-1.svg"
                  alt=""
                  class="inline-block h-16"
                />
                <div class="flex flex-col">
                  <h6 class="text-sm font-bold md:text-base">Jonathan Smith</h6>
                  <p class="text-sm text-[#636262]">Small Business Owner</p>
                </div>
              </div>
              <div class="flex">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
              </div>
            </div>
            <p class="text-[#636262]">
              “Lorem ipsum dolor sit amet, &nbsp;elit ut aliquam, purus sit amet
              luctus venenatis elit ut aliquam, purus sit amet luctus venenatis"
            </p>
          </div>
          <!-- Item -->
          <div
            class="grid min-h-[280px] grid-cols-[1fr_1.75fr] gap-6 rounded-2xl bg-white p-8 md:p-10"
          >
            <!-- Author -->
            <div class="flex flex-col justify-between">
              <div class="flex flex-col items-start gap-4">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c34d_Image%20%26%20Quotation-2.svg"
                  width="90"
                  alt=""
                  class="inline-block h-16"
                />
                <div class="flex flex-col">
                  <h6 class="text-sm font-bold md:text-base">Jonathan Smith</h6>
                  <p class="text-sm text-[#636262]">Small Business Owner</p>
                </div>
              </div>
              <div class="flex">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
              </div>
            </div>
            <p class="text-[#636262]">
              “Lorem ipsum dolor sit amet, &nbsp;elit ut aliquam, purus sit amet
              luctus venenatis elit ut aliquam, purus sit amet luctus venenatis"
            </p>
          </div>
          <!-- Item -->
          <div
            class="grid min-h-[280px] grid-cols-[1fr_1.75fr] gap-6 rounded-2xl bg-white p-8 md:p-10"
          >
            <!-- Author -->
            <div class="flex flex-col justify-between">
              <div class="flex flex-col items-start gap-4">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c34f_Image%20%26%20Quotation-3.svg"
                  alt=""
                  class="inline-block h-16"
                />
                <div class="flex flex-col">
                  <h6 class="text-sm font-bold md:text-base">Jonathan Smith</h6>
                  <p class="text-sm text-[#636262]">Small Business Owner</p>
                </div>
              </div>
              <div class="flex">
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
                <img
                  src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c347_Vector.svg"
                  alt=""
                  class="mr-1 inline-block w-3.5 flex-none"
                />
              </div>
            </div>
            <p class="text-[#636262]">
              “Lorem ipsum dolor sit amet, &nbsp;elit ut aliquam, purus sit amet
              luctus venenatis elit ut aliquam, purus sit amet luctus venenatis"
            </p>
          </div>
        </div>
        <div class="flex flex-col items-center">
          <a href="#" class="mx-auto font-bold text-black">Check all reviews</a>
        </div>
      </div>
    </section>

    <section class="bg-[#c9fd02]">
      <!-- Container -->
      <div
        class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
        data-aos="fade-up"
        data-aos-duration="900"
      >
        <!-- Component -->
        <div class="mx-auto max-w-[1088px]">
          <!-- Header -->
          <div class="mx-auto mb-8 max-w-3xl text-center md:mb-12 lg:mb-16">
            <h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">
              Our Team Members
            </h2>
            <p class="mx-auto mt-4 max-w-[528px] text-[#636262]">
              Lorem ipsum dolor sit amet elit ut aliquam
            </p>
          </div>
          <!-- Team Items -->
          <div
            class="grid grid-cols-1 gap-5 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4"
          >
            <!-- Team Item -->
            <div
              class="mx-auto flex w-4/5 grid-cols-1 flex-col gap-4 justify-self-auto rounded-md py-8"
            >
              <img
                src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c355_image%2012.png"
                alt=""
                class="mx-auto mb-4 inline-block h-40 w-40 flex-none rounded-full object-cover lg:h-48 lg:w-48"
              />
              <div class="flex flex-col items-center">
                <p class="font-bold">John Robert</p>
                <p class="text-center text-sm text-[#636262]">
                  Webflow Developer
                </p>
              </div>
              <div class="mt-4 flex flex-wrap items-center justify-center">
                <a
                  href="#"
                  class="mr-2 inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c348_FacebookLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
                <a
                  href="#"
                  class="inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c346_InstagramLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
              </div>
            </div>
            <!-- Team Item -->
            <div
              class="mx-auto flex w-4/5 grid-cols-1 flex-col gap-4 justify-self-auto rounded-md py-8"
            >
              <img
                src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c35b_image%209.png"
                alt=""
                class="mx-auto mb-4 inline-block h-40 w-40 flex-none rounded-full object-cover lg:h-48 lg:w-48"
              />
              <div class="flex flex-col items-center">
                <p class="font-bold">John Robert</p>
                <p class="text-center text-sm text-[#636262]">
                  Webflow Developer
                </p>
              </div>
              <div class="mt-4 flex flex-wrap items-center justify-center">
                <a
                  href="#"
                  class="mr-2 inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c348_FacebookLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
                <a
                  href="#"
                  class="inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c346_InstagramLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
              </div>
            </div>
            <!-- Team Item -->
            <div
              class="mx-auto flex w-4/5 grid-cols-1 flex-col gap-4 justify-self-auto rounded-md py-8"
            >
              <img
                src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c351_image%2011.png"
                alt=""
                class="mx-auto mb-4 inline-block h-40 w-40 flex-none rounded-full object-cover lg:h-48 lg:w-48"
              />
              <div class="flex flex-col items-center">
                <p class="font-bold">John Robert</p>
                <p class="text-center text-sm text-[#636262]">
                  Webflow Developer
                </p>
              </div>
              <div class="mt-4 flex flex-wrap items-center justify-center">
                <a
                  href="#"
                  class="mr-2 inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c348_FacebookLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
                <a
                  href="#"
                  class="inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c346_InstagramLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
              </div>
            </div>
            <!-- Team Item -->
            <div
              class="mx-auto flex w-4/5 grid-cols-1 flex-col gap-4 justify-self-auto rounded-md py-8"
            >
              <img
                src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c35d_image%2010.png"
                alt=""
                class="mx-auto mb-4 inline-block h-40 w-40 flex-none rounded-full object-cover lg:h-48 lg:w-48"
              />
              <div class="flex flex-col items-center">
                <p class="font-bold">John Robert</p>
                <p class="text-center text-sm text-[#636262]">
                  Webflow Developer
                </p>
              </div>
              <div class="mt-4 flex flex-wrap items-center justify-center">
                <a
                  href="#"
                  class="mr-2 inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c348_FacebookLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
                <a
                  href="#"
                  class="inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c346_InstagramLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
              </div>
            </div>
            <div
              class="mx-auto flex w-4/5 grid-cols-1 flex-col gap-4 justify-self-auto rounded-md py-8"
            >
              <img
                src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c353_image%207.png"
                alt=""
                class="mx-auto mb-4 inline-block h-40 w-40 flex-none rounded-full object-cover lg:h-48 lg:w-48"
              />
              <div class="flex flex-col items-center">
                <p class="font-bold">John Robert</p>
                <p class="text-center text-sm text-[#636262]">
                  Webflow Developer
                </p>
              </div>
              <div class="mt-4 flex flex-wrap items-center justify-center">
                <a
                  href="#"
                  class="mr-2 inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c348_FacebookLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
                <a
                  href="#"
                  class="inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c346_InstagramLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
              </div>
            </div>
            <div
              class="mx-auto flex w-4/5 grid-cols-1 flex-col gap-4 justify-self-auto rounded-md py-8"
            >
              <img
                src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c359_image%2013.png"
                alt=""
                class="mx-auto mb-4 inline-block h-40 w-40 flex-none rounded-full object-cover lg:h-48 lg:w-48"
              />
              <div class="flex flex-col items-center">
                <p class="font-bold">John Robert</p>
                <p class="text-center text-sm text-[#636262]">
                  Webflow Developer
                </p>
              </div>
              <div class="mt-4 flex flex-wrap items-center justify-center">
                <a
                  href="#"
                  class="mr-2 inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c348_FacebookLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
                <a
                  href="#"
                  class="inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c346_InstagramLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
              </div>
            </div>
            <div
              class="mx-auto flex w-4/5 grid-cols-1 flex-col gap-4 justify-self-auto rounded-md py-8"
            >
              <img
                src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c35f_image%208.png"
                alt=""
                class="mx-auto mb-4 inline-block h-40 w-40 flex-none rounded-full object-cover lg:h-48 lg:w-48"
              />
              <div class="flex flex-col items-center">
                <p class="font-bold">John Robert</p>
                <p class="text-center text-sm text-[#636262]">
                  Webflow Developer
                </p>
              </div>
              <div class="mt-4 flex flex-wrap items-center justify-center">
                <a
                  href="#"
                  class="mr-2 inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c348_FacebookLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
                <a
                  href="#"
                  class="inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c346_InstagramLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
              </div>
            </div>
            <div
              class="mx-auto flex w-4/5 grid-cols-1 flex-col gap-4 justify-self-auto rounded-md py-8"
            >
              <img
                src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c357_image%206.png"
                alt=""
                class="mx-auto mb-4 inline-block h-40 w-40 flex-none rounded-full object-cover lg:h-48 lg:w-48"
              />
              <div class="flex flex-col items-center">
                <p class="font-bold">John Robert</p>
                <p class="text-center text-sm text-[#636262]">
                  Webflow Developer
                </p>
              </div>
              <div class="mt-4 flex flex-wrap items-center justify-center">
                <a
                  href="#"
                  class="mr-2 inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c348_FacebookLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
                <a
                  href="#"
                  class="inline-block max-w-full rounded-full border border-solid border-black p-[8px]"
                >
                  <img
                    src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c346_InstagramLogo%20(4).svg"
                    alt=""
                    class="inline-block w-6"
                  />
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section>
      <!-- Container -->
      <div
        class="mx-auto w-full max-w-7xl px-5 pt-16 md:px-10 md:py-24 lg:pb-32"
        data-aos="fade-up"
        data-aos-duration="900"
      >
        <!-- Component -->
        <div class="grid grid-cols-1 gap-20 lg:grid-cols-2">
          <!-- Left Side -->
          <div
            class="mx-auto flex max-w-[720px] flex-col items-center gap-4 text-center"
          >
            <img
              src="https://uploads-ssl.webflow.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c361_Online_math_tutoring.svg"
              alt=""
              class="inline-block"
            />
            <div class="flex flex-col items-center">
              <h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">
                Convenient. Reliable. Power up your payments.
              </h2>
              <p class="mt-4 max-w-[528px] text-[#636262]">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit ut
                aliquam, purus sit amet luctus venenatis, lectus
              </p>
            </div>
          </div>
          <!-- Right Side -->
          <div class="rounded-2xl bg-[#f7f6f2] p-6">
            <div class="mx-auto w-full rounded-2xl bg-white p-8">
              <h3 class="mt-6 text-center text-2xl font-bold md:text-3xl">
                Get a free quote
              </h3>
              <p
                class="mx-auto mb-6 mt-2 max-w-[480px] text-center text-sm text-[#636262] lg:mb-8"
              >
                Lorem ipsum dolor sit amet, consectetur
              </p>
              <!-- Form Div -->
              <div class="mx-auto w-full max-w-[400px]">
                <form method="get">
                  <div class="relative">
                    <label for="name-2" class="mb-1 font-bold">Your Name</label>
                    <input
                      type="text"
                      class="mb-4 block h-9 w-full rounded-md border-[1.5px] border-solid border-[#eceae2] px-3 py-6 text-sm text-[#333333] focus:border-[#3898ec]"
                      maxlength="256"
                      name="name-2"
                      placeholder=""
                      required=""
                    />
                  </div>
                  <div class="relative mb-2">
                    <label for="name-2" class="mb-1 font-bold"
                      >Email Address</label
                    >
                    <input
                      type="email"
                      class="mb-4 block h-9 w-full rounded-md border-[1.5px] border-solid border-[#eceae2] px-3 py-6 text-sm text-[#333333] focus:border-[#3898ec]"
                      maxlength="256"
                      name="name-2"
                      placeholder=""
                      required=""
                    />
                  </div>
                  <div class="relative mb-5 md:mb-6 lg:mb-8">
                    <label for="field-3" class="mb-1 font-bold"
                      >Project Brief</label
                    >
                    <textarea
                      placeholder=""
                      maxlength="5000"
                      name="field"
                      class="mb-2.5 min-h-[128px] w-full rounded-md border-[1.5px] border-solid border-[#eceae2] p-3 text-sm text-[#333333] focus:border-[#3898ec]"
                    >
                    </textarea>
                  </div>
                  <input
                    type="submit"
                    value="Get free quote"
                    class="m-0 inline-block w-full max-w-none cursor-pointer rounded-full border border-solid border-[#c9fd02] bg-[#c9fd02] px-6 py-4 text-center font-bold text-black transition hover:border-black hover:bg-white"
                  />
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section>
      <!-- Container -->
      <div
        class="mx-auto w-full max-w-7xl px-5 pb-16 md:px-10 md:pb-24 lg:pb-32"
        data-aos="fade-up"
        data-aos-duration="900"
      >
        <!-- Component -->
        <div class="flex flex-col items-center">
          <!-- Heading Div -->
          <div class="mb-8 max-w-[800px] text-center md:mb-12 lg:mb-16">
            <h2 class="mb-4 text-3xl font-extrabold md:text-5xl">
              The latest and greatest news
            </h2>
            <p class="mx-auto mt-4 max-w-[528px] text-[#636262]">
              Lorem ipsum dolor sit amet elit ut aliquam
            </p>
          </div>
          <!-- Blog Content -->
          <div
            class="grid w-full grid-cols-1 gap-4 md:grid-cols-2 lg:grid-cols-3"
          >
            <!-- Blog Item -->
            <a
              href="https://neo-saas.webflow.io/blog-posts/7-things-about-web-design-your-boss-wants-to-know"
              class="flex max-w-full flex-col gap-4 rounded-md px-4 md:px-2"
            >
              <img
                alt=""
                src="https://assets.website-files.com/646f6c0e32ec6f9ad7a4504c/646f6c1b66883bd637dfb14a_image9.jpeg"
                class="inline-block h-60 w-full rounded-2xl object-cover"
              />
              <div
                class="flex h-full w-full flex-col items-start justify-around px-0 py-4"
              >
                <div class="mb-4 flex flex-col items-start gap-4">
                  <div class="rounded-md bg-[#f6ad1b] px-2 py-1.5">
                    <p>Marketing</p>
                  </div>
                  <p class="text-xl font-bold md:text-2xl">
                    7 Things About Web Design Your Boss Wants To Know
                  </p>
                </div>
                <!-- Author -->
                <div
                  class="flex flex-col items-start md:flex-row lg:items-center"
                >
                  <p class="text-sm text-[#636262]">Laila Bahar</p>
                  <p class="ml-2 mr-2 hidden text-sm text-[#636262] md:block">
                    -
                  </p>
                  <p class="text-sm text-[#636262]">6 mins</p>
                </div>
              </div>
            </a>
            <!-- Blog Item -->
            <a
              href="https://neo-saas.webflow.io/blog-posts/7-of-the-best-examples-of-beautiful-blog-design"
              class="h-ax-w-full flex flex-col gap-4 rounded-md px-4 md:px-2"
            >
              <img
                alt=""
                src="https://assets.website-files.com/646f6c0e32ec6f9ad7a4504c/646f6c1b66883bd637dfb14e_image14.jpeg"
                class="inline-block h-60 w-full rounded-2xl object-cover"
              />
              <div
                class="flex h-full w-full flex-col items-start justify-around px-0 py-4"
              >
                <div class="mb-4 flex flex-col items-start gap-4">
                  <div class="rounded-md bg-[#f6ad1b] px-2 py-1.5">
                    <p>Docs</p>
                  </div>
                  <p class="text-xl font-bold md:text-2xl">
                    7 of the Best Examples of Beautiful Blog Design
                  </p>
                </div>
                <!-- Author -->
                <div
                  class="flex flex-col items-start md:flex-row lg:items-center"
                >
                  <p class="text-sm text-[#636262]">Laila Bahar</p>
                  <p class="ml-2 mr-2 hidden text-sm text-[#636262] md:block">
                    -
                  </p>
                  <p class="text-sm text-[#636262]">6 mins</p>
                </div>
              </div>
            </a>
            <!-- Blog Item -->
            <a
              href="https://neo-saas.webflow.io/blog-posts/the-history-of-web-design"
              class="hmax-w-full flex flex-col gap-4 rounded-md px-4 md:px-2"
            >
              <img
                alt=""
                src="https://assets.website-files.com/646f6c0e32ec6f9ad7a4504c/646f6c1b66883bd637dfb144_image19.jpeg"
                class="inline-block h-60 w-full rounded-2xl object-cover"
              />
              <div
                class="flex h-full w-full flex-col items-start justify-around px-0 py-4"
              >
                <div class="mb-4 flex flex-col items-start gap-4">
                  <div class="rounded-md bg-[#f6ad1b] px-2 py-1.5">
                    <p>Payment</p>
                  </div>
                  <p class="text-xl font-bold md:text-2xl">
                    The History Of Web Design
                  </p>
                </div>
                <!-- Author -->
                <div
                  class="flex flex-col items-start md:flex-row lg:items-center"
                >
                  <p class="text-sm text-[#636262]">Laila Bahar</p>
                  <p class="ml-2 mr-2 hidden text-sm text-[#636262] md:block">
                    -
                  </p>
                  <p class="text-sm text-[#636262]">6 mins</p>
                </div>
              </div>
            </a>
          </div>
        </div>
      </div>
    </section>

    <footer class="relative text-white">
      <img
        src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f683b1e3793b739a1c34c_Pricing%20BG%20(1).svg"
        alt=""
        class="absolute inset-[0%] -z-[1] inline-block h-full w-full object-cover"
      />
      <!-- Container -->
      <div
        class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
      >
        <!-- Component -->
        <div class="flex flex-col items-center">
          <!-- Logo -->
          <a href="#">
            <img
              src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f66cdeeb4ddfdae25a26c_%5BA%5D--Navbar%20Brand.png"
              alt=""
              class="inline-block h-16"
            />
          </a>
          <p class="mx-auto mt-4 max-w-[528px] text-center text-[#636262]">
            Lorem ipsum dolor sit amet consectetur adipiscing elit ut
            aliquam,purus sit amet luctus magna fringilla urna
          </p>
          <!-- Footer Links -->
          <div class="mt-10 text-center font-semibold">
            <a
              href="#"
              class="inline-block px-6 py-2 text-white transition [border-bottom:1px_solid_rgba(0,_0,_0,_0)] hover:text-white hover:[border-bottom:1px_solid_rgb(201,_253,_2)]"
              >About</a
            >
            <a
              href="#"
              class="inline-block px-6 py-2 text-white transition [border-bottom:1px_solid_rgba(0,_0,_0,_0)] hover:text-white hover:[border-bottom:1px_solid_rgb(201,_253,_2)]"
              >Features</a
            >
            <a
              href="#"
              class="inline-block px-6 py-2 text-white transition [border-bottom:1px_solid_rgba(0,_0,_0,_0)] hover:text-white hover:[border-bottom:1px_solid_rgb(201,_253,_2)]"
              >Works</a
            >
            <a
              href="#"
              class="inline-block px-6 py-2 text-white transition [border-bottom:1px_solid_rgba(0,_0,_0,_0)] hover:text-white hover:[border-bottom:1px_solid_rgb(201,_253,_2)]"
              >Support</a
            >
            <a
              href="#"
              class="inline-block px-6 py-2 text-white transition [border-bottom:1px_solid_rgba(0,_0,_0,_0)] hover:text-white hover:[border-bottom:1px_solid_rgb(201,_253,_2)]"
              >Help</a
            >
          </div>
          <!-- Social Links -->
          <div class="mt-10 flex gap-7 px-6 py-2.5">
            <a
              href="#"
              class="max-w-[24px] text-[#3a3a3a] transition hover:text-[#c9fd02]"
            >
              <svg
                width="40"
                height="41"
                viewBox="0 0 40 41"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M0 20.0176C0 31.0633 8.95431 40.0176 20 40.0176C31.0457 40.0176 40 31.0633 40 20.0176C40 8.97188 31.0457 0.0175781 20 0.0175781C8.95431 0.0175781 0 8.97188 0 20.0176Z"
                  fill="#181818"
                ></path>
                <path
                  d="M12.5938 13.0019C12.9629 12.9588 13.3255 13.1241 13.5352 13.4309C15.0105 15.5897 16.7826 16.4878 18.7489 16.6921C18.8454 15.8509 19.0724 15.0197 19.4991 14.288C20.125 13.2143 21.143 12.4239 22.5972 12.1318C24.6066 11.7282 26.1366 12.4559 27.0244 13.3471L28.8162 13.0122C29.199 12.9406 29.5884 13.0977 29.8144 13.4148C30.0403 13.7319 30.0617 14.1513 29.8691 14.4897L28.1496 17.5118C28.3064 21.8732 27.0944 24.9169 24.5103 27.0139C23.1395 28.1262 21.178 28.7571 19.0249 28.9519C16.855 29.1482 14.4021 28.9108 11.9638 28.1988C11.536 28.0739 11.2425 27.681 11.2441 27.2354C11.2457 26.7897 11.542 26.3989 11.9706 26.277C13.1968 25.9283 14.1301 25.6268 14.9738 25.1003C13.7753 24.464 12.8923 23.6322 12.2673 22.6839C11.3986 21.3658 11.0765 19.8964 11.0125 18.5711C10.9486 17.2459 11.1401 16.0185 11.3418 15.1327C11.4566 14.6285 11.5907 14.1218 11.7755 13.6379C11.9098 13.2891 12.2246 13.0449 12.5938 13.0019Z"
                  fill="currentColor"
                ></path>
              </svg>
            </a>
            <a
              href="#"
              class="max-w-[24px] text-[#3a3a3a] transition hover:text-[#c9fd02]"
            >
              <svg
                width="40"
                height="41"
                viewBox="0 0 40 41"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M0 20.0176C0 31.0633 8.9543 40.0176 20 40.0176C31.0457 40.0176 40 31.0633 40 20.0176C40 8.97188 31.0457 0.0175781 20 0.0175781C8.9543 0.0175781 0 8.97188 0 20.0176Z"
                  fill="#181818"
                ></path>
                <path
                  d="M21.0642 14.2002L21.8087 13.8944C22.4141 13.6533 23.1955 13.409 24.1192 13.5643C26.01 13.8821 27.3145 14.9031 28.0914 16.2573C28.3908 16.7791 28.1489 17.4666 27.5887 17.686C26.6569 18.0509 25.9999 18.9575 25.9999 20.015C25.9999 21.1227 26.7211 22.0647 27.7222 22.3919C28.2405 22.5614 28.5317 23.1367 28.3615 23.6547C27.9201 24.9974 27.2836 26.2363 26.5305 27.2363C25.7871 28.2236 24.879 29.0446 23.868 29.4448C23.2088 29.7058 22.5002 29.6083 21.8227 29.4402L21.4206 29.3332L20.8237 29.1598C20.5528 29.0815 20.2747 29.0133 19.9999 29.0133C19.7251 29.0133 19.447 29.0815 19.1761 29.1598L18.5793 29.3332L18.1772 29.4402C17.4996 29.6083 16.7911 29.7058 16.1319 29.4448C14.8586 28.9408 13.7355 27.7648 12.8874 26.3784C12.0242 24.9673 11.3701 23.2178 11.1034 21.3925C10.8762 19.838 10.9988 18.0935 11.7181 16.6169C12.4589 15.0962 13.8138 13.9117 15.8806 13.5643C16.7204 13.4231 17.4426 13.6121 18.0218 13.8288L18.352 13.9597L18.9357 14.2002C19.3354 14.3568 19.6515 14.449 19.9999 14.449C20.3484 14.449 20.6645 14.3568 21.0642 14.2002ZM19.7677 10.2828C20.744 9.30649 22.2426 9.22214 22.5961 9.5757C22.9497 9.92925 22.8653 11.4278 21.889 12.4041C20.9127 13.3804 19.4141 13.4648 19.0606 13.1112C18.707 12.7577 18.7914 11.2591 19.7677 10.2828Z"
                  fill="currentColor"
                ></path>
              </svg>
            </a>
            <a
              href="#"
              class="max-w-[24px] text-[#3a3a3a] transition hover:text-[#c9fd02]"
            >
              <svg
                width="40"
                height="41"
                viewBox="0 0 40 41"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M0 20.0176C0 31.0633 8.9543 40.0176 20 40.0176C31.0457 40.0176 40 31.0633 40 20.0176C40 8.97188 31.0457 0.0175781 20 0.0175781C8.9543 0.0175781 0 8.97188 0 20.0176Z"
                  fill="#181818"
                ></path>
                <path
                  d="M15.0236 9.80887C15.6422 10.0193 16.4075 10.3546 17.1487 10.8544C18.0469 10.6228 19.0061 10.4983 20.0001 10.4983C20.993 10.4983 21.9513 10.6226 22.8488 10.8537C23.5898 10.3541 24.3549 10.019 24.9733 9.8087C25.6702 9.57176 26.6635 9.18702 27.2532 9.84033C27.6536 10.2839 27.7529 11.0283 27.8243 11.5958C27.9041 12.23 27.9227 13.0567 27.7128 13.8763C28.5157 14.9131 29.0001 16.1507 29.0001 17.4983C29.0001 19.5405 27.894 21.3131 26.2569 22.5409C25.5034 23.106 24.6274 23.5656 23.6667 23.8971C23.8811 24.3874 24.0001 24.929 24.0001 25.4983V28.4983C24.0001 29.0506 23.5523 29.4983 23.0001 29.4983H17C16.4478 29.4983 16 29.0506 16 28.4983V27.507C15.0447 27.624 14.2441 27.5205 13.5626 27.2314C12.8508 26.9294 12.3547 26.461 11.9818 26.0135C11.6281 25.5891 11.2425 24.6332 10.6838 24.447C10.1599 24.2723 9.8767 23.706 10.0513 23.1821C10.226 22.6581 10.7923 22.375 11.3163 22.5496C11.982 22.7715 12.4155 23.2517 12.7132 23.6369C13.1923 24.2568 13.5836 25.0678 14.3437 25.3902C14.6563 25.5228 15.1155 25.6108 15.8323 25.512L16.0001 25.4785C16.0028 24.9164 16.1215 24.3817 16.3334 23.8971C15.3727 23.5656 14.4967 23.106 13.7432 22.5409C12.1061 21.3131 11.0001 19.5405 11.0001 17.4983C11.0001 16.1523 11.4833 14.9159 12.2845 13.8799C12.0738 13.0596 12.0922 12.2321 12.1719 11.5973C12.1735 11.5845 12.1751 11.5717 12.1767 11.5589C12.2496 10.9774 12.3355 10.2921 12.7431 9.84044C13.3327 9.18709 14.3268 9.5719 15.0236 9.80887Z"
                  fill="currentColor"
                ></path>
              </svg>
            </a>
            <a
              href="#"
              class="max-w-[24px] text-[#3a3a3a] transition hover:text-[#c9fd02]"
            >
              <svg
                width="40"
                height="41"
                viewBox="0 0 40 41"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M0 20.0176C0 31.0633 8.95431 40.0176 20 40.0176C31.0457 40.0176 40 31.0633 40 20.0176C40 8.97188 31.0457 0.0175781 20 0.0175781C8.95431 0.0175781 0 8.97188 0 20.0176Z"
                  fill="#181818"
                ></path>
                <path
                  d="M21.5 29.9059C26.3113 29.1821 30 25.0306 30 20.0176C30 14.4947 25.5228 10.0176 20 10.0176C14.4771 10.0176 10 14.4947 10 20.0176C10 25.0306 13.6887 29.1821 18.5 29.9059V23.0176H17C16.1716 23.0176 15.5 22.346 15.5 21.5176C15.5 20.6892 16.1716 20.0176 17 20.0176H18.5V18.0176C18.5 16.0846 20.067 14.5176 22 14.5176H22.5C23.3284 14.5176 24 15.1891 24 16.0176C24 16.846 23.3284 17.5176 22.5 17.5176H22C21.7239 17.5176 21.5 17.7414 21.5 18.0176V20.0176H23C23.8284 20.0176 24.5 20.6892 24.5 21.5176C24.5 22.346 23.8284 23.0176 23 23.0176H21.5V29.9059Z"
                  fill="currentColor"
                ></path>
              </svg>
            </a>
          </div>
        </div>
      </div>
    </footer>

    <section class="relative top-0 h-auto w-full bg-[#101010] lg:w-full">
      <div class="mx-auto flex h-full w-full flex-col items-center p-6">
        <p class="text-base text-[#636262]">
          © Copyright 2021. All rights reserved.
        </p>
      </div>
    </section>
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
