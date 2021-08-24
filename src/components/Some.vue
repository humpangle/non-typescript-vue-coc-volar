<template>
  <div @click="sayHi">{{ msg }}</div>
</template>

<script>
export default {
  name: "some",
  props: {
    msg: String,
    sayHi: {
      type: Function,
      required: true,
    },
  },
};
</script>
