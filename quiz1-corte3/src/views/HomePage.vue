<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Probando</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Login</ion-title>
        </ion-toolbar>
      </ion-header>
      <div id="login-container">
        <div id="login-form">
          <InputGeneric type="input" id="name" name="name" label="Nombre: " />
          <InputGeneric type="date" id="fecha" name="fecha" label="Fecha:" />
          <InputGeneric type="input" id="telefono" name="telefono" label="Telefono:" />
          <InputGeneric type="input" id="correo" name="correo" label="Correo:" />
        </div>
        <div>
          <ButtonGeneric id="agregar" value="agregar" fill="outline" color="primary" />
          <ButtonGeneric id="actualizar" value="actualizar" fill="outline" color="warning" />
        </div>
        <div>
          <InputComponent type="password" id="personaId"  />
          <ButtonGeneric id="consultar" value="consultar" fill="outline" color="success" />
          <ButtonGeneric id="eliminar" value="eliminar" fill="outline" color="danger" />
        </div>
        <div>
          <CardGeneric id = "mensaje" value = "Aprendiendo Front" content= "Es una practica para componentes reutilizables" color="tertiary"/>
        </div>
      </div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import InputGeneric from '@/components/InputGeneric.vue';
import ButtonGeneric from '@/components/ButtonGeneric.vue';
import CardGeneric from '@/components/CardGeneric.vue';
</script>

<style scoped>
#login-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
}

#cart-image {
  margin-bottom: 20px;
  width: 100px;
}

#description {
  margin-bottom: 20px;
  text-align: center;
}

#description p {
  margin: 0;
  padding: 10px; 
}

#login-form {
  max-width: 300px;
  width: 100%;
}
</style>