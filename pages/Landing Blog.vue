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

    <!-- Blog -->
    <section>
      <!-- Container -->
      <div
        class="mx-auto w-full max-w-7xl px-5 py-16 md:px-10 md:py-24 lg:py-32"
      >
        <!-- Component -->
        <div class="flex flex-col items-center">
          <!-- Heading Div -->
          <div class="mb-8 max-w-[800px] text-center md:mb-12 lg:mb-16">
            <h2 class="mb-4 mt-6 text-3xl font-extrabold md:text-5xl">
              The latest and greatest news
            </h2>
            <div class="mx-auto mt-4 max-w-[528px]">
              <p class="text-[#636262]">
                Lorem ipsum dolor sit amet elit ut aliquam
              </p>
            </div>
          </div>
          <!-- Blog Content -->
          <div
            class="grid w-full grid-cols-1 gap-4 md:grid-cols-2 lg:grid-cols-3"
          >
            <!-- Blog Item -->
            <div>
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
                  <div class="flex flex-col items-start">
                    <div
                      class="flex items-start max-[991px]:flex-col lg:items-center"
                    >
                      <p class="text-sm text-[#636262]">Laila Bahar</p>
                      <p
                        class="ml-2 mr-2 text-sm text-[#636262] max-[991px]:hidden"
                      >
                        -
                      </p>
                      <p class="text-sm text-[#636262]">6 mins</p>
                    </div>
                  </div>
                </div>
              </a>
            </div>
            <!-- Blog Item -->
            <div>
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
                  <div class="flex flex-col items-start">
                    <div
                      class="flex items-start max-[991px]:flex-col lg:items-center"
                    >
                      <p class="text-sm text-[#636262]">Laila Bahar</p>
                      <p
                        class="ml-2 mr-2 text-sm text-[#636262] max-[991px]:hidden"
                      >
                        -
                      </p>
                      <p class="text-sm text-[#636262]">3 mins</p>
                    </div>
                  </div>
                </div>
              </a>
            </div>
            <!-- Blog Item -->
            <div>
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
                  <div class="flex flex-col items-start">
                    <div
                      class="flex items-start max-[991px]:flex-col lg:items-center"
                    >
                      <p class="text-sm text-[#636262]">Jake Smith</p>
                      <p
                        class="ml-2 mr-2 text-sm text-[#636262] max-[991px]:hidden"
                      >
                        -
                      </p>
                      <p class="text-sm text-[#636262]">3 mins</p>
                    </div>
                  </div>
                </div>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Footer -->

    <footer class="block bg-black">
      <div
        class="py-16 md:py-24 lg:py-32 mx-auto w-full max-w-7xl px-5 md:px-10"
      >
        <a href="#" class="mb-12 inline-block max-w-full">
          <img
            src="https://assets.website-files.com/646f65e37fe0275cfb808405/646f66cdeeb4ddfdae25a26c_%5BA%5D--Navbar%20Brand.png"
            alt=""
            class="inline-block max-h-10"
          />
        </a>
        <div
          class="grid grid-cols-[auto_1fr] justify-between gap-10 sm:grid-cols-[auto_auto_auto] lg:grid-cols-[0.45fr_auto_auto_auto]"
        >
          <div
            class="flex w-full grid-cols-1 flex-col items-start justify-start gap-8 max-[991px]:mr-0 max-[991px]:max-w-[400px] max-[991px]:[grid-area:span_1/span_3/span_1/span_3] max-[479px]:[grid-area:span_1/span_2/span_1/span_2]"
          >
            <p class="text-[#636262]">
              Lorem ipsum dolor sit amet, &nbsp;elit ut aliquam, purus sit amet
              luctus
            </p>
            <div class="mx-0 mb-4 w-full">
              <form
                name="email-form"
                method="get"
                class="relative flex max-w-full items-center justify-center"
              >
                <input
                  type="email"
                  class="m-0 block h-full max-h-8 w-full rounded-lg border border-solid border-black bg-[#101010] px-3 py-6 align-middle text-sm text-[#333333] focus:border-[#3898ec] focus:outline-0"
                  maxlength="256"
                  name="email-4"
                  placeholder="Enter your email"
                  required=""
                />
                <div
                  class="absolute bottom-[0%] left-[auto] right-[5%] top-[25%] text-[#c9fd02]"
                >
                  <svg
                    width="24"
                    height="25"
                    viewBox="0 0 24 25"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M20.9752 3.02708C20.7866 2.83863 20.5512 2.70382 20.2932 2.63651C20.0353 2.5692 19.764 2.57182 19.5074 2.64411L2.0391 7.57102C1.74519 7.65391 1.48358 7.82454 1.28924 8.0601C1.0949 8.29565 0.977084 8.58491 0.951545 8.88922C0.926006 9.19353 0.993958 9.49838 1.14632 9.76303C1.29868 10.0277 1.52819 10.2395 1.80418 10.3702L9.11045 13.8311L14.1057 8.83591C14.2463 8.69525 14.4371 8.61623 14.636 8.61623C14.835 8.61623 15.0257 8.69525 15.1664 8.83591C15.3071 8.97657 15.3861 9.16735 15.3861 9.36628C15.3861 9.5652 15.3071 9.75598 15.1664 9.89664L10.1712 14.8919L13.6321 22.1981C13.7519 22.4552 13.9429 22.6726 14.1823 22.8246C14.4218 22.9767 14.6997 23.057 14.9834 23.0562C15.0263 23.0562 15.0696 23.0544 15.1131 23.0508C15.418 23.0269 15.708 22.9097 15.9439 22.7151C16.1798 22.5205 16.35 22.258 16.4313 21.9632L21.3582 4.49494C21.4304 4.2383 21.433 3.96707 21.3657 3.7091C21.2984 3.45112 21.1636 3.21572 20.9752 3.02708Z"
                      fill="currentColor"
                    ></path>
                  </svg>
                </div>
                <input
                  type="submit"
                  value="Subscribe"
                  class="absolute bottom-[0%] left-[auto] right-[0%] top-[0%] m-0 inline-block cursor-pointer rounded-[60px] border border-solid border-[#c9fd02] bg-[#c9fd02] px-6 py-4 text-center font-bold text-black no-underline opacity-0 transition hover:border-black hover:bg-white"
                />
                <div></div>
                <div></div>
              </form>
            </div>
            <div>
              <p class="font-bold uppercase text-[#c9fd02]">email us</p>
              <p class="text-[#636262]">support@flowspark.co</p>
            </div>
          </div>
          <div class="flex flex-col items-start font-semibold no-underline">
            <div class="m-4 max-[991px]:ml-0 max-[991px]:mr-0">
              <p class="text-xl text-white">Solution</p>
            </div>
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Marketing</a
            >
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Analytics</a
            >
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Commerce</a
            >
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Insights</a
            >
          </div>
          <div class="flex flex-col items-start font-semibold no-underline">
            <div class="m-4 max-[991px]:ml-0 max-[991px]:mr-0">
              <p class="text-xl text-white">Support</p>
            </div>
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Pricing</a
            >
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Documentation</a
            >
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Guides</a
            >
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >API&nbsp;Status</a
            >
          </div>
          <div class="flex flex-col items-start font-semibold no-underline">
            <div class="m-4 max-[991px]:ml-0 max-[991px]:mr-0">
              <p class="text-xl text-white">Company</p>
            </div>
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >About</a
            >
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Blog</a
            >
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Jobs</a
            >
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Press</a
            >
            <a
              href="#"
              class="py-2 text-sm font-bold text-[#636262] transition hover:text-white"
              >Partners</a
            >
          </div>
        </div>
        <div
          class="mb-20 mt-20 w-full border border-solid border-[#101010]"
        ></div>
        <div
          class="flex flex-row justify-between max-[991px]:items-center max-[767px]:flex-col max-[767px]:items-start max-[479px]:flex-col-reverse"
        >
          <div class="max-[991px]:flex-none">
            <p class="text-[#636262]">© Copyright 2021. All rights reserved.</p>
          </div>
          <div
            class="text-center font-semibold max-[991px]:ml-0 max-[991px]:mr-0 max-[991px]:py-1"
          >
            <a
              href="#"
              class="inline-block py-2 font-bold text-[#636262] transition hover:text-white max-[479px]:px-2.5 lg:pl-12 pl-5 pr-0"
              >Terms of Service</a
            >
            <a
              href="#"
              class="inline-block py-2 font-bold text-[#636262] transition hover:text-white max-[479px]:px-2.5 lg:pl-12 pl-5 pr-0"
              >License</a
            >
            <a
              href="#"
              class="inline-block py-2 font-bold text-[#636262] transition hover:text-white max-[479px]:px-2.5 lg:pl-12 pl-5 pr-0"
              >Privacy Policy</a
            >
          </div>
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
