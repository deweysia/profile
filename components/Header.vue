<template>
  <div class="flex flex-wrap items-center mb-16">
    <div class="mr-4">
      <img
        class="h-36 w-36 object-cover rounded-full shadow-lg transition duration-200 transform hover:scale-110"
        src="https://scontent.fmnl4-6.fna.fbcdn.net/v/t31.0-8/24059720_1598991790161508_483327100315942203_o.jpg?_nc_cat=107&ccb=2&_nc_sid=174925&_nc_ohc=8oPsNe_yrQUAX-kJdnv&_nc_ht=scontent.fmnl4-6.fna&oh=d1046244443be09a402511683b26c3ac&oe=6037724D"
        alt="Dewey Sia"
      >
    </div>
    <div>
      <h1 class="text-5xl font-bold text-gray-900 leading-normal">
        Dewey Sia
      </h1>
      <div class="mb-6 text-gray-600">
        Full-Stack Developer based in Toronto, Canada.
      </div>
      <Navigation />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Navigation from './Navigation.vue'
export default Vue.extend({
  components: {
    Navigation
  }
})
</script>
<style>

</style>
