<template>
  <div>
    <h2>{{ title }}</h2>
    counter: {{ $store.state.counter.counter}}
    <button v-on:click="$store.commit('counter/countUp')">+1</button>
    <button v-on:click="$store.commit('counter/resetCount')">RESET!!!!!</button>
  </div>
</template>

<script>
export default {
  data: function(){
    return {
      title: 'Counter App'
    }
  }
}
</script>

<style scoped>

</style>
