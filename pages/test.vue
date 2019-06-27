<template>
  <button @click="test()"></button>
</template>

<script>
export default {
  methods: {
    test() {
      this.$store.dispatch("getProducts");
    }
  }
};
</script>

<style>
</style>
