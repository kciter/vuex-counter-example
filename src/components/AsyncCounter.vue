<template>
  <div>
    <button @click="increment">
      비동기 증가
    </button>
  </div>
</template>

<script>
  export default {
    name: 'AsyncCounter',
    methods: {
      increment () {
        this.$store.dispatch('asyncIncrement')
        // store의 asyncIncrement action을 실행합니다
      }
    }
  }
</script>