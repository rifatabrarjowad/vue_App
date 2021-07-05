<template>
  <div>
    <h1>Hello From Home component</h1>
    <button @click="hello">Hello from home</button>
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
  },
};
</script>
