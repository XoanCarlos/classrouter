<template>
  <div class="row">
    <div class="col-md-12">
      <h4>Articulos a la Venta</h4>
      <p v-for="articulo in articulos" :key="articulo.id">
        <router-link :to=" {
          name: 'Fruta',
          params: { id: articulo.id, producto: articulo.producto, precio: articulo.precio }
        }">
          {{articulo.id}}. {{articulo.producto}}
        </router-link></p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      articulos: [
        {id: 1, producto: 'naranjas', precio: '1.25'},
        {id: 2, producto: 'platanos', precio: '0.95'},
        {id: 3, producto: 'kiwis', precio: '1.95'},
        {id: 4, producto: 'cerezas', precio: '2.25'},
        {id: 5, producto: 'zanahorias', precio: '0.75'},
        {id: 6, producto: 'ciruelas', precio: '1.75'}
      ]
    }
  }
}
</script>

<style scoped>

</style>