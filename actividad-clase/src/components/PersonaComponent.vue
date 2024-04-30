<template>
    <InputComponent id="id" name="id" type="hidden" />
    <InputComponent id="primerNombre" name="primerNombre" label="Primer Nombre:" />
    <InputComponent id="segundoNombre" name="segundoNombre" label="Segundo Nombre:" />
    <InputComponent id="primerApellido" name="primerApellido" label="Primer Apellido:" />
    <InputComponent id="segundoApellido" name="segundoApellido" label="SegundoApelldi:" />
    <InputComponent id="tipoDocumento" name="tipoDocumento" label="Tipo Documento: " />
    <InputComponent type="number" id="Documento" name="Documento" label="Documento: " />
</template>

<script setup lang="ts">
import InputComponent from './InputComponent.vue';
</script>

<style scoped src="../theme/container.css"></style>