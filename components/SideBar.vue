<template>
  <div>
    <div style="background-color: #745FFE;" class="text-gray-100 flex justify-between md:hidden">
      <!-- logo -->
      <a href="#" class="block p-4 text-white font-bold">Anvik Singh</a>

      <!-- mobile menu button -->
      <button @click="openSideBarForSmallScreens" class="mobile-menu-button p-4 focus:outline-none focus:bg-gray-700">
        <svg class="h-5 w-5" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      </button>
    </div>

    <!-- sidebar -->
    <div style="background: #F9FAFC;height: 100vh;" class="sidebar text-black-100 w-64 space-y-6 py-7 px-2 absolute inset-y-0 left-0 transform -translate-x-full md:relative md:translate-x-0 transition duration-200 ease-in-out">

      <!-- logo -->
      <a href="#" class="text-black flex items-center space-x-2 px-4">
        <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4M7.835 4.697a3.42 3.42 0 001.946-.806 3.42 3.42 0 014.438 0 3.42 3.42 0 001.946.806 3.42 3.42 0 013.138 3.138 3.42 3.42 0 00.806 1.946 3.42 3.42 0 010 4.438 3.42 3.42 0 00-.806 1.946 3.42 3.42 0 01-3.138 3.138 3.42 3.42 0 00-1.946.806 3.42 3.42 0 01-4.438 0 3.42 3.42 0 00-1.946-.806 3.42 3.42 0 01-3.138-3.138 3.42 3.42 0 00-.806-1.946 3.42 3.42 0 010-4.438 3.42 3.42 0 00.806-1.946 3.42 3.42 0 013.138-3.138z" />
        </svg>
        <span class="text-xl font-extrabold flex items-center">
          <span>Anvik Singh</span>
          <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-0.5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
          </svg>
        </span>
      </a>

      <!-- nav -->
      <nav>
        <a href="#" class="block py-2 px-4 rounded transition duration-200 hover-bg-custom-color bg-custom-color-selected hover:text-white">
          History
        </a>
        <a href="" class="block py-2 px-4 rounded transition duration-200 hover-bg-custom-color hover:text-white">
          Dashboard
        </a>
        <a href="" class="block py-2 px-4 rounded transition duration-200 hover-bg-custom-color hover:text-white">
          Payments
        </a>
        <a href="" class="block py-2 px-4 rounded transition duration-200 hover-bg-custom-color hover:text-white">
          Cards
        </a>
        <a href="" class="block py-2 px-4 rounded transition duration-200 hover-bg-custom-color hover:text-white">
          Accounts
        </a>
        <a href="" class="block py-2 px-4 rounded transition duration-200 hover-bg-custom-color hover:text-white">
          Cards
        </a>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SideBar',
  data() {
    return {
    
    }
  },
  methods: {
    openSideBarForSmallScreens() {
      const sidebar = document.querySelector(".sidebar");
      sidebar.classList.toggle("-translate-x-full");
    }
  }
}
</script>

<style scoped>
.hover-bg-custom-color:hover {
  background-color: #745FFE;
}
.bg-custom-color-selected {
  background-color: #745FFE;
  color: white;
}
</style>
