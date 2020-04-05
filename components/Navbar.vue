<template>
<header class="z-10 w-full h-12 py-1 px-6 flex shadow text-white text-xl font-medium">
  <nuxt-link to="/" class="text-3xl brand z-20">R</nuxt-link>

  <ul class="hidden p-1 justify-around w-3/5 m-auto md:flex">
    <li class="hover:underline">
      <nuxt-link to="/">Home</nuxt-link>
    </li>
    <li class="hover:underline">
      <nuxt-link to="/">About Us</nuxt-link>
    </li>
    <li class="hover:underline">
      <nuxt-link to="/">Blog</nuxt-link>
    </li>
    <li class="hover:underline">
      <nuxt-link to="/">Contact</nuxt-link>
    </li>
    <li class="hover:underline">
      <nuxt-link to="/register">Register</nuxt-link>
    </li>
    <li class="hover:underline">
      <nuxt-link to="/login">Login</nuxt-link>
    </li>
  </ul>

  <ul class="m-auto z-10 dropdown overflow-hidden w-0 opacity-0 h-0 p-3 duration-300 flex flex-col absolute inset-0 z-0 justify-center bg-red-600 text-center" id="dropdown">
    <li class="p-3 hover:underline" @click='expand'>
      <nuxt-link to="/">Home</nuxt-link>
    </li>
    <li class="p-3 hover:underline" @click='expand'>
      <nuxt-link to="/">About Us</nuxt-link>
    </li>
    <li class="p-3 hover:underline" @click='expand'>
      <nuxt-link to="/">Blog</nuxt-link>
    </li>
    <li class="p-3 hover:underline" @click='expand'>
      <nuxt-link to="/">Contact</nuxt-link>
    </li>
    <li class="p-3 hover:underline" @click='expand'>
      <nuxt-link to="/register">Register</nuxt-link>
    </li>
    <li class="p-3 hover:underline" @click='expand'>
      <nuxt-link to="/login">Login</nuxt-link>
    </li>
  </ul>
  <button class="ml-auto z-10 w-6 border-none outline-none text-white block md:hidden" @click="expand">
    <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="bars" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" class="svg-inline--fa fa-bars fa-w-14 fa-3x">
      <path fill="currentColor"
        d="M16 132h416c8.837 0 16-7.163 16-16V76c0-8.837-7.163-16-16-16H16C7.163 60 0 67.163 0 76v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16z"
        class="">
      </path>
    </svg>
  </button>
</header>
</template>
<script>
export default {
  mounted() {
    window.addEventListener("resize", (e) => {
      let width = e.target.window.innerWidth;
      if (width > 768) {
        let menu = document.getElementById('dropdown');
        if (menu.classList.contains('opacity-100')) {
          this.expand();
        }
      }
    }, true);
  },
  data() {
    return {

    }
  },
  methods: {
    expand(e) {
      let menu = document.getElementById('dropdown');
      menu.classList.toggle('h-0');
      menu.classList.toggle('h-full');
      menu.classList.toggle('pt-16');
      menu.classList.toggle('opacity-0');
      menu.classList.toggle('opacity-100');
      menu.classList.toggle('w-0');
      menu.classList.toggle('w-screen');
    }
  }
}
</script>
