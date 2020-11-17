<template>
  <ion-item
      class="w-full"
      lines="inset"
  >
    <ion-label position="stacked">
      One
    </ion-label>
    <div class="flex w-full">
      <ion-input type="text"/>
    </div>
  </ion-item>
  <ion-item
      class="w-full"
      lines="inset"
  >
    <ion-label position="stacked">
      Two
    </ion-label>
    <ion-input type="text"/>
  </ion-item>
  <ion-item
      class="w-full"
      lines="inset"
  >
    <ion-label position="stacked">
      Three
    </ion-label>
    <ion-input type="text"/>
  </ion-item>
  <ion-item
      class="w-full"
      lines="inset"
  >
    <ion-label position="stacked">
      Four
    </ion-label>
    <ion-input type="text"/>
  </ion-item>
  <ion-item
      class="w-full"
      lines="inset"
  >
    <ion-label position="stacked">
      Five
    </ion-label>
    <ion-input type="text"/>
  </ion-item>
  <ion-item
      lines="inset"
      class="w-full"
  >
    <ion-label position="stacked">
      Six
    </ion-label>
    <ion-textarea class="px-2"/>
  </ion-item>
</template>
<script lang="ts">
import { IonInput, IonItem, IonLabel, IonTextarea } from '@ionic/vue'

export default {
  name: 'Fields',

  components: {
    IonInput,
    IonItem,
    IonLabel,
    IonTextarea
  }
}
</script>
<style scoped>
.w-full {
  width: 100%;
}

.flex {
  display: flex;
}

.px-2 {
  padding-left: 8px;
  padding-right: 8px;
}

</style>
