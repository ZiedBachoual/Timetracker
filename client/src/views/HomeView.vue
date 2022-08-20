<template>
  <div class="home">
    <HelloWorld msg/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import HelloWorld from '@/components/HelloWorld.vue' // @ is an alias to /src

export default defineComponent({
  name: 'HomeView',
  components: {
    HelloWorld
  }
})
const maDate: Date = new Date()
const msg = maDate.getDate() + '/' + (maDate.getMonth() + 1) + '/' + maDate.getFullYear() + ' ' + maDate.getHours() + ':' + maDate.getMinutes() + ':' + maDate.getSeconds()
</script>
