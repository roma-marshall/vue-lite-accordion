<template>
  <main>
    <div class="relative overflow-hidden rounded"
         :class="darkmode ? 'text-gray-300 bg-slate-800' : 'text-slate-900 bg-gray-100'">
      <input type="checkbox" class="peer absolute top-0 inset-x-0 w-full h-16 opacity-0 z-10 cursor-pointer mb-20">
      <div class="flex my-5 mx-10 px-3"
           :class="'justify-' + position">
        <h1 class="text-xl">{{ head }}</h1>
      </div>
      <!-- arrow icon -->
      <div class="absolute top-6 right-5 transition-transform duration-500 rotate-0 peer-checked:rotate-180">
        <svg
            class="h-6 w-6"
            :class="darkmode ? 'stroke-gray-300' : 'stroke-slate-900'"
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"/>
        </svg>
      </div>
      <!-- Content -->
      <div class="overflow-hidden transition-all duration-500 max-h-0 peer-checked:max-h-screen">
        <div class="mb-5 pt-3 px-3 mx-1 sm:mx-10 border-t">
          <p>{{ body }}</p>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'RomaAccordion',
  props: {
    head: String,
    body: String,
    darkmode: String,
    position: String
  }
}
</script>

<style scoped>

</style>
