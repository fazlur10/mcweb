<template>
  <nav class="bg-white md:flex md:justify-between md:items-center md:px-4 md:py-3">
    <div class="flex items-center justify-between px-4 py-3 md:p-0 max-h-20 min-h-12 lg:mx-20">
      <div>
        <img class="h-16" src="~/assets/img/mc_logo.png" alt="Millennium Concept" />
      </div>
      <div class="md:hidden">
        <button
          @click="isOpen = !isOpen"
          type="button"
          class="block text-violet-600 hover:text-violet-400 focus:text-violet-400 focus:outline-none"
        >
          <svg class="h-6 w-6 fill-current" viewBox="0 0 24 24">
            <path v-if="isOpen" fill-rule="evenodd" d="M18.278 16.864a1 1 0 0 1-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 0 1-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 0 1 1.414-1.414l4.829 4.828 4.828-4.828a1 1 0 1 1 1.414 1.414l-4.828 4.829 4.828 4.828z"/>
            <path v-if="!isOpen" fill-rule="evenodd" d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z" />
          </svg>
        </button>
      </div>
    </div>
    <div :class="isOpen ? 'block' : 'hidden'" class="px-2 pt-2 pb-4 md:flex">
      <a href="#" class="block px-2 py-1 text-violet-600 font-semibold rounded hover:bg-violet-500 hover:text-violet-50">Why Digital X</a>
      <a href="#" class="mt-1 block px-2 py-1 text-violet-600 font-semibold rounded hover:bg-violet-500 hover:text-violet-50 md:mt-0 md:ml-2">Solutions</a>
      <a href="#" class="mt-1 block px-2 py-1 text-violet-600 font-semibold rounded hover:bg-violet-500 hover:text-violet-50 md:mt-0 md:ml-2">About Us</a>
      <a href="#" class="mt-1 block px-2 py-1 text-violet-600 font-semibold rounded hover:bg-violet-500 hover:text-violet-50 md:mt-0 md:ml-2">Contact Us</a>
      <a href="#" class="mt-1 block px-2 py-1 md:px-6 md:py-3.5 text-white font-semibold rounded bg-violet-500 hover:text-violet-50   md:hover:text-violet-500 md:hover:bg-white md:bg-violet-500 md:rounded-3xl md:-mt-2.5 md:ml-2">+65 8248 1167</a>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false
    };
  },
  methods: {
    toggleNavbar: function() {
      this.showMenu = !this.showMenu;
    }
  }
};
</script>
