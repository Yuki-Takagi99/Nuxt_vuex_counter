<template>
  <div>
    <h2>{{ title }}</h2>
    counter: {{ $store.state.counter.counter}}
    <button v-on:click="$store.commit('counter/countUp')">+1</button>
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
