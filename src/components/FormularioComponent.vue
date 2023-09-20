<template>
  <div class="box">
    <div class="columns">
      <div
        class="column is-8"
        role="form"
        aria-label="Formulário para criação de uma nova tarefa"
      >
        <input
          type="text"
          class="input"
          placeholder="Qual tarefa você deseja iniciar?"
        />
      </div>
      <div class="column">
        <div
          class="is-flex is-align-items-center is-justify-content-space-between"
        >
        </div>
    </div>
  </div>
  </div>
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
