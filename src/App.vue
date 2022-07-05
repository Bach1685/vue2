<template>
  <div id="app">
    <MyComponent :text="text" @inc="inc" />
    <input type="text" v-model="cunt" />
    <p>cunt: {{ cunt }}</p>
  </div>
</template>

<script>
import MyComponent from "./components/MyComponent.vue";

export default {
  name: "App",
  components: {
    MyComponent,
  },
  data() {
    return {
      text: "Hello",
      cunt: "",
    };
  },
  methods: {
    inc() {
      console.log("сработало событие!");
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
