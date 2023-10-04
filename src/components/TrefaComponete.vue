
import Cronometro from './Cronometro.vue';
<template>
    <div class="box has-text-weight-bold">
        <div class="columns">
            <div class="column is-7">
                Descrição da Tarefa
            </div>
            <div class="column">
                <CronometroTimer TempoEmSegundos="15"/>
            </div>
        </div>
    </div>
</template>
<script lang="ts">

import  {defineComponent} from 'vue'
import CronometroTimer from './Cronometro.vue';

export default defineComponent ({
    name:'TarefaVue',
    components: {
        CronometroTimer,
    }

})
</script>