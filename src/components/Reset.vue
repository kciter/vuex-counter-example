<template>
  <div>
    <button @click="reset">
      리셋
    </button>
  </div>
</template>

<script>
  export default {
    name: 'Reset',
    methods: {
      reset () {
        this.$store.commit('RESET')
      }
    }
  }
</script>