<template>
  <HelloWorld />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import {provide, ref} from 'vue';
export default {
  name: 'App',
  components: {
    HelloWorld
  },
  setup() {
    let name = ref('张三');
    provide('xd', name)
    return {

    }
  }
}
</script>

<style>
</style>
