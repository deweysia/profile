<template>
  <div class="flex flex-wrap text-gray-600">
    <nuxt-link
      v-for="n in navigation"
      :key="n.link"
      class="mr-4 text-xs font-semibold uppercase hover:text-blue-500"
      :to="n.link"
    >{{ n.name }}</nuxt-link>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data () {
    return {
      navigation: [
      {name: 'About Me', link:'/'},
      {name: 'Work', link:'/work'},
      {name: 'Experience', link:'/experience'},
      {name: 'Skills', link:'#'},
      {name: 'Blog', link:'#'}]
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
  transition: 0.25s ease;
}
a:hover:after {
  width: 100%;
}

a.nuxt-link-exact-active:after {
  content:'';
  border-bottom: 2px solid #4299e1;
  width: 100%;
}

a.nuxt-link-exact-active {
  @apply text-blue-500;
}
</style>
