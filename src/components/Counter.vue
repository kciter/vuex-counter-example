<template>
  <div>
    <button @click="increment">증가</button>
    <button @click="decrement">감소</button>
  </div>
</template>

<script>
  export default {
    name: 'Counter',
    methods: {
      increment () {
        this.$store.commit('INCREMENT')
        // store 객체의 INCREMENT mutation을 실행합니다.
      },
      decrement () {
        this.$store.commit('DECREMENT')
        // store 객체의 DECREMENT mutation을 실행합니다.
      }
    }
  }
</script>