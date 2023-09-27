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
          v-model="descricao"
        />
      </div>
      <div class="column">
        <div
          class="is-flex is-align-items-center is-justify-content-space-between"
        ></div>
      </div>
    </div>
  </div>
  <div class="box">
    <div class="columns">
      <TemporizadorVue @aoTemporizadorFinalizado="finalizarTarefa" />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import TemporizadorVue from "./TemporizadorComponete.vue";

export default defineComponent({
  name: "FormularioVue",
  components: {
    TemporizadorVue,
  },
  data() {
    return {
      descricao: "",
    };
  },
  methods: {
    finalizarTarefa(tempoDecorrido: number): void {
      console.log("tempo da tarefa", tempoDecorrido);
      console.log("descrição da tarefa", this.descricao);
      this.descricao = "";
    },
  },
});
</script>
