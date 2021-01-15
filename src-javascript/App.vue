<script>

import {ref} from "vue";
import Component from "./Component.vue";

export default {
  name: 'App',
  components: {
    Component,
  },
  setup() {
    const toggle1 = ref(false);
    const toggle2 = ref(true);
    return {
      toggle1,
      toggle2,
    };
  }
};
</script>

<template>
  <div><button @click="toggle1 = !toggle1">toggle1 (default false)</button></div>
  <div>Component (toggle1): <Component v-if="toggle1" key="1"></Component></div>
  <div><button @click="toggle2 = !toggle2">toggle2 (default true)</button></div>
  <div>Component (toggle2): <Component v-if="toggle2" key="2"></Component></div>
</template>
