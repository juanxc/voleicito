<template>
  <section id="cuadroprincipal">
    <article class="container">
      <div v-for="lugar in lugares" class="cont-photo row">
        <div class="col-md-8">
          <figure>
            <img
              src="~/assets/canchas/lospinos.jpg"
              class="figure-img img-fluid rounded"
              alt="Los Pinos"
            />
          </figure>
        </div>
        <div class="col-md-4">
          <ul class="list-group">
            <li class="list-group-item active cabecera-lugar">
              {{ lugar.nombre }}
            </li>
            <li class="list-group-item text-left">
              Martes/Jueves/Domingo {{ lugar.horadesde }} - {{ lugar.horahasta }}
            </li>
            <li class="list-group-item text-left">{{ lugar.direccion }}</li>
            <li class="list-group-item text-left">Nivel Barrio</li>
          </ul>
        </div>
      </div>
    </article>
  </section>
</template>

<script>
import axios from 'axios'
export default {
  name: "lugar",
  data(){
    return{
      lugares: [],
      errors: []
    }
  },
  mounted(){
    //this.lugares = [{nombre: 'los pinos', direccion: 'av principal'}];
    axios.get('http://localhost:4000/api')
    .then(response=>{
      this.lugares = response.data
    })
    .catch(e=>{
      this.errors.push(e)
    })
  }
}
</script>
