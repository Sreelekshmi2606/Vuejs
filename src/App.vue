<template>
  <DockMenu :items="items">
  </DockMenu>
</template>

<script>
import { DockMenu } from "vue-dock-menu";
import "vue-dock-menu/dist/vue-dock-menu.css";

export default {
  name: "ExampLe",
  components: {
    DockMenu
  },
  data() {
    return {
      items: [
        {
          name: "Home",
          menu: [{ name: "About" }, { name: "News", }, { name: "Gallary" }]
        },
        {
          name: "Products",
          menu: [{ name: "Vegetables" }, {
            name: "Fruits",
            menu: [{ name: "Orange" }, { name: "Apple" }]
          }, { name: "Sweets" }]
        }
      ]
    }
  }
}
</script>





<!-- <template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
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
</style> -->
