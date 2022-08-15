<template>
  <div>
    <div class="absolute top-5 right-5 p-5">
      <svg id="moon" class="h-6 w-6 text-gray-500 cursor-pointer" fill="none" stroke="currentColor" viewbox="0 0 24 24">
        <path d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"/>
      </svg>
      <svg class="h-6 w-6 text-gray-200 cursor-pointer hidden" id="sun" fill="none" viewbox="0 0 24 24" stroke="currentColor">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z" />
      </svg>
    </div>
    <div class="min-h-screen flex justify-center items-center bg-gray-100 dark:bg-gray-800">
      <form class="p-10 bg-white dark:bg-gray-700 rounded flex justify-center items-center flex-col shadow-md">
        <p class="mb-5 text-3xl uppercase text-gray-600 dark:text-gray-300 select-none uppercase">{{ component_name }}</p>
        <input type="email" name="email" class="mb-5 p-3 w-80 focus:border-blue-700 rounded border-2 outline-none dark:bg-transparent dark:border-gray-400 dark:text-gray-300" autocomplete="off" placeholder="Email" />
        <input type="password" name="password" class="mb-5 p-3 w-80 focus:border-blue-700 rounded border-2 outline-none dark:bg-transparent dark:border-gray-400 dark:text-gray-300" autocomplete="off" placeholder="Password" />
        <button class="bg-blue-500 text-white px-10 py-2 w-full rounded hover:bg-transparent hover:text-blue-500 hover:border-blue-500 border-2 border-transparent dark:hover:text-white" id="login" type="submit"><span>Login</span></button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      component_name: 'Login',
    }
  }
}
</script>