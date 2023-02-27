<template>
  <div class = 'row'>
    <div class = 'cod-md-12'>
      <h5>Fruta del Día</h5>
    </div>
    <div class = 'col-md-6'>
      <p>Id Fruta: {{ $route.params.id}} </p>
      <p>Fruta: {{ $route.params.producto}}</p>
      <p>Precio: {{ $route.params.precio}}</p>
    </div>
  </div>
</template>
