<template>
<div class="container m-auto">
  <div class="max-w-lg rounded overflow-hidden shadow-xl mx-auto bg-white">
    <div class="px-6 py-4">
      <div class="font-bold text-xl mb-2 text-center">Register</div>
      <div class="flex flex-col mt-8 pb-6">
        <div class="flex flex-col sm:flex-row">
          <label for="username" class="text-center whitespace-no-wrap sm:text-left">Username :</label>
          <input type="text" name="username" id="username" class="ml-2 appearance-none border rounded w-full duration-300 text-gray-700 leading-tight focus:outline-none p-1 focus:border-gray-400" />
        </div>
        <div class="flex flex-col mt-4 sm:flex-row">
          <label for="email" class="text-center whitespace-no-wrap sm:text-left">Email :</label>
          <input type="email" name="email" id="email" class="ml-2 appearance-none border rounded w-full duration-300 text-gray-700 leading-tight focus:outline-none p-1 focus:border-gray-400" />
        </div>
        <div class="flex flex-col mt-4 sm:flex-row">
          <label for="password" class="text-center whitespace-no-wrap sm:text-left">Password :</label>
          <input type="password" name="password" id="password" class="ml-2 appearance-none border rounded w-full duration-300 text-gray-700 leading-tight focus:outline-none p-1 focus:border-gray-400" />
        </div>
        <div class="flex flex-col mt-4 sm:flex-row">
          <label for="confirm-password" class="text-center whitespace-no-wrap sm:text-left">Confirm Password :</label>
          <input type="password" name="confirm-password" id="confirm-password" class="ml-2 appearance-none border rounded w-full duration-300 text-gray-700 leading-tight focus:outline-none p-1 focus:border-gray-400" />
        </div>
      </div>
      <button class="fancy-red py-1 px-4 block m-auto rounded text-white duration-300 fancy-btn hover:shadow">Register</button>
    </div>
  </div>
</div>
</template>
