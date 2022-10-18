<template>
  <ion-page id="page">
    <ion-tabs >
      <ion-router-outlet ></ion-router-outlet>
      <ion-tab-bar style="color:red;" slot="bottom">
        <ion-tab-button style=" background-color:orangered" tab="tab1" href="/tabs/tab1">
          <ion-icon :icon="grid" />
          <ion-label></ion-label>
        </ion-tab-button>
          
        <ion-tab-button style=" background-color:orangered" tab="tab2" href="/tabs/tab2">
          <ion-icon :icon="person" />
          <ion-label></ion-label>
        </ion-tab-button>
        
        <ion-tab-button style=" background-color:orangered" tab="tab3" href="/tabs/tab3">
          <ion-icon :icon="reader" />
          <ion-label></ion-label>
        </ion-tab-button>

        <ion-tab-button style=" background-color:orangered" tab="tab4" href="/tabs/tab4">
          <ion-icon :icon="home" style/>
          <ion-label></ion-label>
        </ion-tab-button>

      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonTabBar, IonTabButton, IonTabs, IonLabel, IonIcon, IonPage, IonRouterOutlet } from '@ionic/vue';
import { home, grid, person, reader } from 'ionicons/icons';

export default defineComponent({
  name: 'TabsPage',
  components: { IonLabel, IonTabs, IonTabBar, IonTabButton, IonIcon, IonPage, IonRouterOutlet },
  setup() {
    return {
      person,
      home,
      grid, 
      reader
    }
  }
});
</script>

<style scoped> 
  #page{
    background-color: white;
  }
</style>