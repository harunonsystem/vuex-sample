<template>
  <div class="count">
      <h1>This is an count page</h1>
      <h5>クリックすると数字変わるよ(´・ω・`)</h5>
      {{ $store.state.count }}
      <button @click="increment">+</button>
      <button @click="decrement">-</button>
  </div>
</template>

<script>
export default {
    methods: {
        increment() {
            this.$store.commit("increment");
        },
        decrement() {
            this.$store.commit("decrement");
        }
    }
}
</script>

<style>

</style>