<template>
    <ion-page>
      <ion-header :translucent="true">
        <ion-toolbar>
          <ion-title>Empleado</ion-title>
        </ion-toolbar>
      </ion-header>  
      <ion-content>       
        <div id="login-container">  
          <div id="login-form">
            <PersonaComponent />         
          </div>
  
          <div> 
            <CrudButtonComponent />
          </div>          
        </div>
      </ion-content>
    </ion-page>
  </template>
  
  <script setup lang="ts">
  import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
  import CrudButtonComponent from '@/components/CrudButtonComponent.vue';
  import PersonaComponent from '@/components/PersonaComponent.vue';
  </script>
  
  <style scoped src="../theme/container.css"></style>