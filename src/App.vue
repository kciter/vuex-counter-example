<template>
  <div id="app">
    카운트: {{ $store.state.count }}

    <counter></counter>
    <reset></reset>
    <async-counter></async-counter>
  </div>
</template>

<script>
  import Counter from './components/Counter'
  import Reset from './components/Reset'
  import AsyncCounter from './components/AsyncCounter'

  export default {
    name: 'app',
    components: {
      Counter,
      Reset,
      AsyncCounter
    }
  }
</script>

<style>
</style>
