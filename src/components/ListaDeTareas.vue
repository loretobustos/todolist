<template>
<div>
    <h1>Lista de Tareas</h1>

    <form>
        <label for="">Tareas</label>
        <input type="text" v-model="tarea">
        <button @click.prevent="agregar_tarea">Añade</button>
    </form>
    <ul>
        <li v-for="tarea in lista_tareas" :key="tarea">
            {{ tarea}}
        </li>
        <button @click.prevent="eliminar_tarea">Eliminar</button>
    </ul>



</div>
</template>

<script>
export default {
    name: 'Lista_de_tareas',
    // props: {},
    data: function(){
        return {
            mensaje:'hola mundo',
            tarea: '',
            lista_tareas: [],
        }
    },
    name: 'Lista_de_tareas',
    // props: {},
    data: function(){
        return {
            mensaje:'hola mundo',
            tarea: '',
            eliminar_tarea: [],
        }
    },
    // computed: {},
    methods: {
        // -- Metodos
        agregar_tarea (){
            alert(this.tarea)
            this.lista_tareas.push(this.tarea)
        },
        eliminar_tarea (){
            alert(this.tarea)
              this.eliminar_tarea.pop(this.tarea)
        }
    }

    // components: {},
}
</script>

<style scoped>

</style>