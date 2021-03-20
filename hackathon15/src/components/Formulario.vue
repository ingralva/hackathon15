<template>

    <div align="center">
        <div class="card" style="width: 400px; padding:10px 20px" >
        <h1>{{title}}</h1>
        <form @submit.prevent="getInformationUser">
            <div class="field" st>
                <label class="label">Id video</label>
                <div class="control">
                    <input 
                        type="text"
                        id="id"
                        placeholder="Id Video"
                        v-model="video.id"
                        class="input"
                    >
                </div>
            </div>
            <div class="field" st>
                <label class="label">Titulo video</label>
                <div class="control">
                    <input 
                        type="text"
                        id="titulo"
                        placeholder="Titulo Video"
                        v-model="video.titulo"
                        class="input"
                    >
                </div>
            </div>
            <div class="field" st>
                <label class="label">Descripción vudeo</label>
                <div class="control">
                    <input 
                        type="text"
                        id="descripcion"
                        placeholder="Descripcion Video"
                        v-model="video.descripcion"
                        class="input"
                    >
                </div>
            </div>
            
            <div>
                <input type="submit" value=Enviar class="button is-success">
            </div>
            
        </form>
        <!-- {{video}} -->
    </div> 
</div> 
</template>

<script>
export default {
    name: 'Formulario',
    props:{
        title:String
    },
    data() {
        return {
            video: {
                id: 0,
                titulo: '',
                visitas: 0,
                descripcion: ''
            }
        }
    },
    methods: {
        getInformationUser(){
            console.log(this.video)
        }
    }
}
</script>

<style>

</style>