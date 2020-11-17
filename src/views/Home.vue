<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Input test</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content>
      <div class="form flex w-full ion-padding-vertical">
        <ion-button @click="showModal = true">Modal</ion-button>

        <ion-modal :is-open="showModal">
          <Modal @close-modal="showModal = false" />
        </ion-modal>

        <Fields/>

      </div>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonButton, IonContent, IonHeader, IonModal, IonPage, IonTitle, IonToolbar } from '@ionic/vue'
import { defineComponent, ref } from 'vue'
import Modal from '@/views/Modal.vue'
import Fields from '@/views/Fields.vue'

export default defineComponent({
  name: 'Home',

  components: {
    Fields,
    Modal,
    IonButton,
    IonContent,
    IonHeader,
    IonModal,
    IonPage,
    IonTitle,
    IonToolbar
  },

  setup() {
    const showModal = ref(false)

    return {
      showModal
    }
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

ion-textarea.bordered {
  border-width: 1px;
  border-color: var(--ion-color-step-250, #c8c7cc);
}
</style>
