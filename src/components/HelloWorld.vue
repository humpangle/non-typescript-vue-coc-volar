<template>
  <app-some :say-hi="sayHi" :msg="msg"></app-some>
</template>

<script>
import { defineComponent } from "@vue/composition-api";
import VueCompositionAPI from '@vue/composition-api'
import Some from "./Some.vue";

Vue.use(VueCompositionAPI);

export default defineComponent({
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
});
</script>
