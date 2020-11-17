<template>
  <div class="w-full h-full">
    <ion-header>
      <ion-toolbar>
        <ion-title>Input modal</ion-title>
        <ion-buttons slot="end">
          <ion-button @click="onDone">Done</ion-button>
        </ion-buttons>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding w-full h-full">
      <Fields/>
    </ion-content>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { IonButton, IonButtons, IonContent, IonHeader, IonTitle, IonToolbar} from '@ionic/vue'
import Fields from './Fields.vue'

export default defineComponent({
  name: 'Modal',

  components: {
    Fields,
    IonButton,
    IonButtons,
    IonContent,
    IonHeader,
    IonTitle,
    IonToolbar
  },

  emits: ['close-modal'],

  setup(props, context) {
    function onDone() {
      console.log('done')
      context.emit('close-modal')
    }

    return {
      onDone
    }
  }
})
</script>

<style scoped>
.w-full {
  width: 100%;
}

.h-full {
  height: 100%;
}

.flex {
  display: flex;
}

</style>
