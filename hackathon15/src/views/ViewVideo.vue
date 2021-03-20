<template>
<div class="" align="center">
  <Titulo
    titulo="Detalles de video"
  />
  <h1>Video - {{$route.params.id}}</h1>

<div class="card" style="width: 400px; padding: 5px;" >
            
            <div class="card-content">
                <div class="media">
                <div class="media-left">
                    <figure class="image is-48x48">
                    <img src="../assets/fondo-video.jpg" alt="Placeholder image">
                    </figure>
                </div>
                <div class="media-content">
                    <p class="title is-4">{{video.titulo}}</p>
                    <p class="subtitle is-6">{{video.visitas}} Visitas</p>
                </div>
                </div>

                <div class="content">
                {{video.descripcion}}                
                </div>
            </div>
        </div>

</div>

  
</template>

<script>

import Titulo from '../components/Titulo.vue'

export default {
    name: 'ViewVideo',
    components: { Titulo },
    data() {
        return {
            video:{}
        };
    },
    methods: {
        async getVideo() {
            const info = await fetch(`http://localhost:3000/videos/${this.$route.params.id}`)
            const data = await info.json();
            this.video = data;
            console.log(data);
        }
    },
    created() {
        this.getVideo();
    }
}
</script>

<style>

</style>