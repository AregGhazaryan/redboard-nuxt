<template>
  <div class="container m-auto">
    <div class="max-w-sm rounded overflow-hidden shadow-xl mx-auto bg-white">
      <div class="px-6 py-4">
        <div class="font-bold text-xl mb-2 text-center">Welcome!</div>
        <p class="text-gray-700 text-base text-center">
          Please sign up or login to continue.
        </p>
      </div>
      <div class="px-6 py-4 flex justify-between">
        <nuxt-link to="/register" class="bg-indigo-500 text-white px-3 py-1 rounded-full transition duration-200 ease-in-out  hover:bg-indigo-400">Register</nuxt-link>
        <nuxt-link to="/login" class="text-white px-3 py-1 rounded-full transition duration-200 ease-in-out fancy-btn">Login</nuxt-link>
      </div>
    </div>
  </div>
</template>
