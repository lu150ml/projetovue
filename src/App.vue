<template>
  <main class="columns is-gapless is-multiline">
    <div class="column is-one-quarter">
        <BarraLateral />
      </div>
      <div class="column is-three-quarter">
      <FormularioVue />
      <div class="lista">
        <TarefaVue />
        <TarefaVue />
        <TarefaVue />
        <TarefaVue />
      </div>
    </div>
  </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraLateral from './components/BarraLateral.vue';
import FormularioVue from './components/FormularioComponent.vue';
import TarefaVue from './components/TrefaComponete.vue';

export default defineComponent({
    name: 'App',
    components: {
      BarraLateral,
      FormularioVue,
      TarefaVue
    }
});
</script>

<style>

</style>
