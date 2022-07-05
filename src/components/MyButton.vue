<template>
  <button @click="click"></button>
</template>

<script>
export default {
  methods: {
    click() {
      console.log("вызвалось внутри компонента");
      this.$emit("click");
    },
  },
};
</script>

<style>
</style>