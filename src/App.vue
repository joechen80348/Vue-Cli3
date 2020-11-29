<template>
  <TitleComponent :title="title">
  </TitleComponent>
  <InputComponent :text.sync="title"></InputComponent>
  <img
    alt="Vue logo"
    src="./assets/logo.png"
  />
  <HelloWorld msg="Welcome to Your Vue.js App" />
</template>

<script>
  import HelloWorld from "./components/HelloWorld.vue";
  import TitleComponent from "./components/Title.vue";
  import InputComponent from "./components/InputComponent/index.vue";

  export default {
    name: "App",
    data() {
      return {
        title: "Hello World",
      };
    },
    components: {
      HelloWorld,
      TitleComponent,
      InputComponent,
    },
    // methods: {
    //   changeHandler(val) {
    //     this.title = val;
    //   },
    // },
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
