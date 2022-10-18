<template >
  <div id="carga"> 
    <ion-app>
      <ion-router-outlet  />
    </ion-app>
  </div>
</template>

<script lang="ts">
import { IonApp, IonRouterOutlet } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {
    IonApp,
    IonRouterOutlet
  }
});
</script>
<style> 
#carga {
  margin: 0;    padding: 0;   -webkit-font-smoothing: antialiased;   -moz-osx-font-smoothing: grayscale;   text-align: center;   background-color: white;   min-height: 100vh; 
}
</style>