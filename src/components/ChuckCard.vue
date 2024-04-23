<template>
    <div class="col-md-4 mb-4">
      <div class="card">
        <img :src="iconUrl" class="card-img-top" alt="Chuck Norris">
        <div class="card-body">
          <p class="card-text">{{ value }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      iconUrl: String,
      value: String
    }
  }
  </script>
  
  <style scoped>
  /* Estilos específicos del componente aquí si es necesario */
  </style>
  
  