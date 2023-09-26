<template>
  
    <ion-chip>Default</ion-chip>
    <ion-chip :disabled="true">Disabled</ion-chip>
    <ion-chip :outline="true">Outline</ion-chip>
    <div>
        <ion-chip>
    <ion-avatar>
      <img alt="Silhouette of a person's head" src="https://ionicframework.com/docs/img/demos/avatar.svg" />
    </ion-avatar>
    <ion-label>Avatar Chip</ion-label>
    <ion-icon :icon="closeCircle"></ion-icon>
  </ion-chip>

  <ion-chip>
    <ion-icon :icon="pin" color="primary"></ion-icon>
    <ion-label>Icon Chip</ion-label>
    <ion-icon :icon="close"></ion-icon>
  </ion-chip>
  <ion-chip>Default</ion-chip>
  <ion-chip color="primary">Primary</ion-chip>
  <ion-chip color="secondary">Secondary</ion-chip>
  <ion-chip color="tertiary">Tertiary</ion-chip>
  <ion-chip color="success">Success</ion-chip>
  <ion-chip color="warning">Warning</ion-chip>
  <ion-chip color="danger">Danger</ion-chip>
  <ion-chip color="light">Light</ion-chip>
  <ion-chip color="medium">Medium</ion-chip>
  <ion-chip color="dark">Dark</ion-chip>
    </div>
  </template>
  
  <script lang="ts">
    import { IonChip, IonAvatar, IonLabel, IonIcon } from '@ionic/vue';
  import { close, closeCircle, pin } from 'ionicons/icons';
  import { defineComponent } from 'vue';
  
    export default defineComponent({
      components: { IonChip, IonAvatar, IonLabel, IonIcon },
      setup() {
      return {
        close,
        closeCircle,
        pin,
      };
    },
    });
  </script>