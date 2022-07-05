<template>
  <div>
    {{ text }}
    <button @click="inc">инкрементировать</button>
    <p>counter: {{ count }}</p>
  </div>
</template>

<script>
export default {
  //   props: ["text"],
  props: {
    text: {
      require: true,
    },
    count: {
      require: true,
      type: Number,
    },
  },
  // data() {
  //   return {
  //     count: 0,
  //   };
  // },
  methods: {
    inc() {
      this.$emit("inc");
    },
  },
};
</script>

<style>
</style>