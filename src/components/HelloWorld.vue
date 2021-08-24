<template>
  <app-some :say-hi="sayHi" :msg="msg"></app-some>
</template>

<script>
import Some from "./Some.vue";

export default {
  name: "HelloWorld",
  components: {
    "app-some": Some,
  },
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
