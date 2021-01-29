<template>
  <header class="rounded-xl hover:bg-indigo-700">
    <nav
      class="flex items-center justify-between h-24 px-6"
      x-data="{ showMenu: false }"
    >
      <a href="#" class="text-xl font-extrabold text-white md:w-1/4">
        tails<span class="text-red-500">.</span>
      </a>

      <div
        class="flex flex-col w-full h-full text-sm lg:text-base md:flex-row md:w-3/4"
      >
        <!-- links -->
        <div
          class="flex flex-col items-center justify-center md:mt-6 md:text-indigo-200 md:w-2/3 md:flex-row"
        >
          <a
            href="#"
            class="inline-block px-4 mx-2 font-medium md:px-0 lg:mx-3 md:hover:text-white"
            >Home</a
          >
          <a
            href="#"
            class="inline-block px-4 mx-2 font-medium md:px-0 lg:mx-3 md:hover:text-white"
            >Features</a
          >
          <a
            href="#"
            class="inline-block px-4 mx-2 font-medium md:px-0 lg:mx-3 md:hover:text-white"
            >Blog</a
          >
          <a
            href="#"
            class="inline-block px-4 mx-2 font-medium md:px-0 lg:mx-3 md:hover:text-white"
            >Contact</a
          >
        </div>

        <!-- sign in sign up -->
        <div
          class="flex flex-col items-center justify-end md:flex-row md:w-1/3"
        >
          <a
            href="#"
            class="text-indigo-200 md:mr-3 hover:text-white lg:mr-5 md:px-4 md:py-2 md:hover:bg-indigo-100 md:rounded-full md:hover:text-indigo-700"
            >Sign in</a
          >
          <a
            href="#"
            class="font-medium md:transition md:duration-150 md:ease-in-out md:text-indigo-600 md:bg-indigo-100 md:border md:border-transparent md:rounded-full md:px-4 md:py-2 whitespace-nowrap hover:bg-white focus:border-indigo-700 focus:ring-indigo-300 focus:outline-none"
            >Sign up</a
          >
        </div>
      </div>

      <!-- note: the below div has which is set to be circular and flex properties are used to center it -->
      <!-- hidden in md: screen -->
      <div
        x-on:click="showMenu = !showMenu"
        class="flex items-center justify-center w-10 h-10 rounded-full cursor-pointer md:hidden"
        x-bind:class="{
          'text-indigo-700 hover:bg-gray-200': showMenu,
          'text-indigo-200 hover:bg-indigo-700':!showMenu
          }"
      >
        <svg
          class="w-6 h-6"
          x-show="!showMenu"
          fill="none"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          viewBox="0 0 24 24"
          stroke="currentColor"
          x-cloak
        >
          <path d="M4 6h16M4 12h16M4 18h16"></path>
        </svg>
        <svg
          class="w-6 h-6"
          x-show="showMenu"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
          x-cloak
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M6 18L18 6M6 6l12 12"
          ></path>
        </svg>
      </div>
    </nav>
  </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>