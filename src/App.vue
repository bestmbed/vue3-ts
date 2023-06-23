<template>
  <dev>
    <h1>App.vue</h1>
    <span> #Debug: {{ count1 }} </span> <br>
    <span> #Debug: {{ count2 }} </span> <br>
  </dev>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  setup() {
    let count1 = 10;
    const count2 = ref<number>(2)
    return {
      count1,
      count2,
    };
  },

});
</script>
