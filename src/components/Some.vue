<template>
  <div @click="sayHi">{{ msg }}</div>
</template>

<script>
import { defineComponent } from "@vue/composition-api";

export default defineComponent({
  name: "some",
  props: {
    msg: String,
    sayHi: {
      type: Function,
      required: true,
    },
  },
});
</script>
