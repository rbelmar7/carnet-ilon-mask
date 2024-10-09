<template>
    <div class="carnet">
      <div class="carnet-header">
        <h1>Carnet de Identidad</h1>
      </div>
      <div class="carnet-body">
        <p><strong>RUN:</strong> {{ run }}</p>
        <p><strong>Apellidos:</strong> {{ apellidos }}</p>
        <p><strong>Nombres:</strong> {{ nombres }}</p>
        <p><strong>Nacionalidad:</strong> {{ nacionalidad }}</p>
        <p><strong>Sexo:</strong> {{ sexo }}</p>
        <p><strong>Fecha de Nacimiento:</strong> {{ fechaNacimiento }}</p>
        <p><strong>Número de Documento:</strong> {{ numeroDocumento }}</p>
        <p><strong>Fecha de Emisión:</strong> {{ fechaEmision }}</p>
        <p><strong>Fecha de Vencimiento:</strong> {{ fechaVencimiento }}</p>
      </div>
    </div>
  </template>
  
  <script>
  import { ref } from 'vue';
  
  export default {
    setup() {

      const run = ref('22.222.222-2');
      const apellidos = ref('MUSK');
      const nombres = ref('JELON REEVE');
      const nacionalidad = ref('Sudafricano');
      const sexo = ref('Masculino');
      const fechaNacimiento = ref('01/01/1990');
      const numeroDocumento = ref('12345678');
      const fechaEmision = ref('01/01/2020');
      const fechaVencimiento = ref('01/01/2030');

      return {
        run,
        apellidos,
        nombres,
        nacionalidad,
        sexo,
        fechaNacimiento,
        numeroDocumento,
        fechaEmision,
        fechaVencimiento
      };
    }
  };
  </script>
  
  <style scoped>
  .carnet {
    width: 300px;
    border: 2px solid #000;
    padding: 20px;
    border-radius: 10px;
    font-family: Arial, sans-serif;
    background-color: #f9f9f9;
  }
  
  .carnet-header {
    text-align: center;
    margin-bottom: 20px;
  }
  
  .carnet-body p {
    margin: 5px 0;
  }
  
  .carnet-body strong {
    color: #333;
  }
  </style>
  