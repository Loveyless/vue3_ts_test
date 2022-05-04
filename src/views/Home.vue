<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App" />

    {{ a }}
  </div>
</template>



<script lang="ts">
import HelloWorld from "@/components/HelloWorld.vue";
import { ref, defineComponent } from "vue";
export default defineComponent({
  setup() {
    let a = ref<number>(1);

    a.value = "哈哈";

    return {
      a,
    };
  },
  components: {
    HelloWorld,
  },
});
</script>
