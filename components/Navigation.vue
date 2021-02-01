<template>
  <div class="flex flex-wrap text-gray-600">
    <a
      v-for="n in navigation"
      :key="n"
      class="mr-4 text-xs font-semibold uppercase hover:text-blue-500"
      href="#"
    >{{ n }}</a>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data () {
    return {
      navigation: ['About Me', 'Work', 'Experience', 'Skills', 'Blog']
    }
  }
})
</script>

<style scoped>
a {
  display: inline-block;
}
a:after {
  content: "";
  display: block;
  border-bottom: 2px solid #4299e1;
  width: 0;
  transition: 0.5s ease;
}
a:hover:after {
  width: 100%;
}
</style>
