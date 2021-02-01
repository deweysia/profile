<template>
  <div class="bg-indigo-100">
    <div class="p-14 h-screen relative m-auto md:w-8/12 bg-white shadow-xl">
      <Header />
      <div class="text-gray-600 font-light">
        <Nuxt />
      </div>
      <Footer />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Header from '../components/Header.vue'
import Footer from '../components/Footer.vue'
export default Vue.extend({
  components: {
    Header,
    Footer
  }
})
</script>
<style>

</style>
