<template>
  <div class="box">
    <div class="columns">
        <TemporizadorVue />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import TemporizadorVue from "./TemporizadorComponete.vue";

export default defineComponent({
  name: "FormularioVue",
  components: {
    TemporizadorVue
  }
});
</script>
