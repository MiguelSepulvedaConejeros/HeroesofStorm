<template>
  <v-container class="container">
    <v-row class="description">
        <h1>Desafia las expectativas de los MOBA</h1>
        <p>Epicos heroes y accion sin cesar en multples campos de batalla</p>
        <v-btn class="btn-heroes">Ver Heroes</v-btn>
    </v-row>
  </v-container>
  <v-alert class="desp-heroes" v-model="alert" border="start" close-label="Close Alert" variant="tonal">!Te damos la bienvenida al Nexo¡!En este reino entre reinos, todo es posible¡ Elige entre decenas de heroes legendarios de todo el panteón de Blizzard, personaloza sus talentos y habilidades en medio del combate y lucha en una infinidad de campos de batalla que redefinen el genero. ¡Esto no es un MOBA promedio, esto es Heroes of the Storm¡</v-alert>
  </template>

<script> 
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'HomeView',

  components: {
  },
});
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  width:35%;
  margin-top:100px;
  border: 3px solid gray;
}
.description {
  display:flex;
  flex-direction: column;
  color: white;
  padding: 15px;
}
.description h1, .description p {
  margin-bottom: 10px;
}
.btn-heroes {
  margin-top:10px;
  margin-bottom:10px;
  width: 25%;
  background-color: #EF6C00;
  align-self: center;
}
.desp-heroes {
  margin-top: 100px;
  height: 150px;
  font-size: 20px;
  color: white;
  background-color:#6A1B9A;
  background-color: rgba(106, 27, 154, 0.5);
}
</style>