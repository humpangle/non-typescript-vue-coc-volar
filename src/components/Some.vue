<template>
  <div @click="sayHi">{{ msg }}</div>
</template>

<script>
import { defineComponent } from "@vue/composition-api";
import VueCompositionAPI from "@vue/composition-api";

Vue.use(VueCompositionAPI);

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
