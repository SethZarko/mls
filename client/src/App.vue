<script lang="ts">
  export default {
    data() {
      return {
        helloWorld: ''
      }
    },
    watch: {
      helloWorld(newState, oldState) {
        if(newState) {
          console.log('State Changed');
        }
      }
    },
    methods: {
      hello() {
        this.helloWorld = 'Hello, World'
      }
    },
    mounted(){
      this.hello()
    }
  }
</script>

<template>
  <h1 class="text-3xl font-bold underline">{{ helloWorld }}</h1>
</template>
