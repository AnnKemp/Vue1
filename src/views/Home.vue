<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src
// some new types
//tuple type = fixed array with predefined data types
//Enum type = allows you to define friendly names to a set of values vb: enum ArrowKeys{
//  Up, Down, Left, Right
//}

export default defineComponent({
  name: "Home",
  components: {
    HelloWorld
  }
});
</script>
