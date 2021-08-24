<template>
  <div @click="sayHi">{{ msg }}</div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  methods: {
    sayHi() {
      console.log("hi");
    },
  },
};
</script>
