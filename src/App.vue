<template>
  <!-- <div>{{ greeting(name) }}</div> -->
  <div>{{ name }}</div>
  <input type="text" v-bind:value="name" />
  <button class="btn btn-primary" v-on:click="chaneName">Click</button>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    let name = ref("hanu");

    // const greeting = (name) => {
    //   return "hello, " + name;
    // };

    const chaneName = () => {
      console.log("chaneName...");
      name.value = "coker";
    };

    return {
      name,
      // greeting,
      chaneName,
    };
  },
};
</script>

<style>
.name {
  color: red;
}
</style>
