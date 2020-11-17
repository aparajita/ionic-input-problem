<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Input test</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content>
      <div class="form flex w-full ion-padding-vertical">
        <ion-item
            class="w-full"
            lines="inset"
        >
          <ion-label position="stacked">
            One
          </ion-label>
          <div class="flex w-full">
            <ion-input type="text" />
          </div>
        </ion-item>

        <ion-item
            class="w-full"
            lines="inset"
        >
          <ion-label position="stacked">
            Two
          </ion-label>
          <ion-input type="text" />
        </ion-item>

        <ion-item
            class="w-full"
            lines="inset"
        >
          <ion-label position="stacked">
            Three
          </ion-label>
          <ion-input type="text" />
        </ion-item>

        <ion-item
            class="w-full"
            lines="inset"
        >
          <ion-label position="stacked">
            Four
          </ion-label>
          <ion-input type="text" />
        </ion-item>

        <ion-item
            class="w-full"
            lines="inset"
        >
          <ion-label position="stacked">
            Five
          </ion-label>
          <ion-input type="text" />
        </ion-item>

        <ion-item
            lines="inset"
            class="w-full"
        >
          <ion-label position="stacked">
            Six
          </ion-label>
          <ion-textarea />
        </ion-item>

        <ion-item
            lines="inset"
            class="w-full"
        >
          <ion-label position="stacked">
            Seven
          </ion-label>
          <ion-textarea class="px-2" />
        </ion-item>
      </div>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonContent, IonHeader, IonInput, IonItem, IonLabel, IonPage, IonTextarea, IonTitle, IonToolbar } from '@ionic/vue'
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Home',
  components: {
    IonContent,
    IonHeader,
    IonInput,
    IonItem,
    IonLabel,
    IonPage,
    IonTextarea,
    IonTitle,
    IonToolbar
  }
});
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

.form {
  flex-direction: column;
  justify-content: space-between;
  align-items: start;
  padding-right: 16px;
}

.px-2 {
  padding-left: 8px;
  padding-right: 8px;
}

ion-textarea.bordered {
  border-width: 1px;
  border-color: var(--ion-color-step-250, #c8c7cc);
}
</style>
