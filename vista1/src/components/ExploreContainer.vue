<template id="template">
  <img id="imagen" src="/assets/foto.png">
  <div id="container" >
    
    <ion-page >
      <H1>
        <ion-title style="font-size: 40px ">Samuel Sanchez</ion-title>
      </H1>
      
      <p id="p">alumno ing informatica</p> 
      <div id="caja">

        <ion-text style="color:black; font-size:20px"> asignaturas</ion-text>
        <br />
        <br />
        <ion-button id="boton1" color="tertiary">Calculo 3</ion-button>
        <ion-button id="boton2" color="medium">ALgebra 2</ion-button>
        <br />
        <ion-button id="boton3" color="success">Inteligencia Artificial</ion-button>

      </div>
    </ion-page>
    
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'ExploreContainer',
  props: {
    name: String
  }
});
 
</script>

<style scoped>
#container {
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  top: 48%;
  transform: translateY(-45%);
  background-color: rgba(255, 255, 255, 0.815);
  height: 93%;
  width:100%;
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container h1 {
  
  line-height: 70px;
  color: #0a0a0a;
  margin: 0;
}

#p{
  color: black;
  font-size:23px;

}
#caja{
  height: 50%;
  width: 75%;
  background-color: white;
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  top: 42%;
  transform: translateY(100%);
  transform: translateX(17%);
}
#boton1
{
  height: 50%;
  width: 45%;
  padding: 3%;
  background-color:medium;
}
#boton2{
  height: 50%;
  width: 45%;
  padding: 3%;
  background-color: medium;
}
#boton3{
  height: 35%;
  width: 75%;
  background-color: medium;
}
#imagen{
  height: 28%;
  width: 50%;
  transform: translateY(55%);
  

}

</style>
