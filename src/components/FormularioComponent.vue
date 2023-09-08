<template>
    <div class="box">
        <div class="columns">
            <div class="columns is-8" role="form" aria-label="Formulario para criação de uma nova tarfea">
                <input type="text" class="input" placeholder="Qual tarefa voce deja iniciar">
            </div>
            <div class="columns">
                <div class="is-flex is align-items-center is-justify-contetnt-space-beteween">
                    <section>
                        <strong>00:00:00</strong>
                    </section>
                    <button class="button">
                        <span class="icon">
                            <i class="fas fa-play"></i>
                        </span>
                        <span>play</span>
                    </button>
                    <button class="button">
                        <span class="icon">
                            <i class="fas fa-stop"></i>
                        </span>
                        <span>stop</span>
                    </button>
                </div>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    name: 'FormularioVue'
})
</script>