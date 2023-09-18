<template>
  <div
    class="columns is-8"
    role="form"
    aria-label="Formulario para criação de uma nova tarfea"
  >
    <input
      type="text"
      class="input"
      placeholder="Qual tarefa você deseja iniciar"
    />
  </div>
  <div class="columns">
    <div class="is-flex is-align-items-center is-justify-content-space-between">
      <CronometroTimer :tempoEmSegundos="tempoEmSegundos" />
      <button class="button" @click="iniciar">
        <span class="icon">
          <i class="fas fa-play"></i>
        </span>
        <span>play</span>
      </button>
      <button class="button" @click="finalizar">
        <span class="icon">
          <i class="fas fa-stop"></i>
        </span>
        <span>stop</span>
      </button>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import CronometroTimer from "./Cronometro.vue";

export default defineComponent({
  name: "TemporizadorVue",
  components: {
    CronometroTimer,
  },
  data() {
    return {
      tempoEmSegundos: 0,
      cronometro: 0,
    };
  },
  methods: {
    iniciar() {
      //começar a  contagem
      // 1 seg = 100ms
      this.cronometro = setInterval(() => {
        this.tempoEmSegundos += 1;
      }, 1000);
    },
    finalizar() {
      clearInterval(this.cronometro);
    },
  },
});
</script>