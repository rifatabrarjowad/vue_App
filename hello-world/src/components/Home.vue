<template>
  <div>
    <h1>Hello From Home component</h1>
    <button @click="hello">Hello from home</button>
    <h1 v-if="show">if</h1>
    <h1 v-else>else</h1>
    <button v-on:click="display">toogle</button>
  </div>
</template>
<script>
export default {
  name: "Home",
  props: {
    data: String,
    msg: String,
  },
  methods: {
    hello() {
      console.warn("alert from hello funtion");
    },
    display() {
      this.show = !this.show;
    },
  },
  data() {
    return {
      show: false,
    };
  },
};
</script>
