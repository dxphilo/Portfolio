<template>
  <div class="bg-bgwhite text-txcolor">
    <!-- component -->
    <div class="header sticky top-0 z-50">
      <!-- Text shadow utilities will be cool -->
      <nav class="flex justify-around pt-4 items-center mb-1 font-bold">
        <div>
          <a href="/" class="flex text-normal pl-10">
            <span class="text-2xl pl-3">John Philip</span>
          </a>
        </div>

        <ul class="list-reset flex text-xl">
          <li class="pr-3">
            <!-- <button v-if="!darkMode" @click="toggleSwitch">
              <svg
                width="1em"
                height="1em"
                viewBox="0 0 24 24"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <circle
                  cx="11.9998"
                  cy="11.9998"
                  r="5.75375"
                  fill="currentColor"
                />
                <g>
                  <circle
                    cx="3.08982"
                    cy="6.85502"
                    r="1.71143"
                    transform="rotate(-60 3.08982 6.85502)"
                    fill="currentColor"
                  />
                  <circle
                    cx="3.0903"
                    cy="17.1436"
                    r="1.71143"
                    transform="rotate(-120 3.0903 17.1436)"
                    fill="currentColor"
                  />
                  <circle
                    cx="12"
                    cy="22.2881"
                    r="1.71143"
                    fill="currentColor"
                  />
                  <circle
                    cx="20.9101"
                    cy="17.1436"
                    r="1.71143"
                    transform="rotate(-60 20.9101 17.1436)"
                    fill="currentColor"
                  />
                  <circle
                    cx="20.9101"
                    cy="6.8555"
                    r="1.71143"
                    transform="rotate(-120 20.9101 6.8555)"
                    fill="currentColor"
                  />
                  <circle
                    cx="12"
                    cy="1.71143"
                    r="1.71143"
                    fill="currentColor"
                  />
                </g>
              </svg>
            </button>
            <button v-else @click="toggleSwitch">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="1em"
                height="1em"
                viewBox="0 0 50 50"
              >
                <path
                  d="M 43.81 29.354 C 43.688 28.958 43.413 28.626 43.046 28.432 C 42.679 28.238 42.251 28.198 41.854 28.321 C 36.161 29.886 30.067 28.272 25.894 24.096 C 21.722 19.92 20.113 13.824 21.683 8.133 C 21.848 7.582 21.697 6.985 21.29 6.578 C 20.884 6.172 20.287 6.022 19.736 6.187 C 10.659 8.728 4.691 17.389 5.55 26.776 C 6.408 36.163 13.847 43.598 23.235 44.451 C 32.622 45.304 41.28 39.332 43.816 30.253 C 43.902 29.96 43.9 29.647 43.81 29.354 Z"
                  fill="currentColor"
                />
              </svg>
            </button> -->
          </li>
          <li>
            <nuxt-link to="/" class="p-2 md:p-4"> Home </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/blog" class="p-2 md:p-4"> Blog </nuxt-link>
          </li>
        </ul>
      </nav>
    </div>
    <div class="relative">
      <Nuxt />
      <Footer />
    </div>
  </div>
</template>
<script>
import Vue from 'vue'

export default Vue.extend({
  data() {
    return {
      darkMode: true,
    }
  },
})
</script>

<style>
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: 'Cormorant Garamond', serif;
  background-color: #f8f9fa;
  color: #1a6183;
}
.header {
  font-size: 19px;
  height: 70px;
  font-weight: 400;
  letter-spacing: 0.25px;
  background-color: #f8f9fa;
  color: #1a6183;
}
ul li {
  background-color: transparent;
  padding-top: 5px;
  line-height: 19px;
  text-decoration: none;
}
</style>
