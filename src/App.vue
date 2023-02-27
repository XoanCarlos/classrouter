<template>
  <div>
    <nav class = 'navbar navbar-ligth bg-ligth'>
      <div class = 'container'>
        <router-link class="navbar-brand" to="/">inicio</router-link>
        <router-link class="navbar-brand" to="/articulos">articulos</router-link>
        <router-link class="navbar-brand" to="/nosotros">nosotros</router-link>
      </div>
     </nav>
    <body>
       <div class="container">
         <table class="table table-bordered">
           <thead>
           <tr>
             <router-view/>
           </tr>
           </thead>
         </table>
       </div>
    </body>
  </div>
</template>

<script>
  export default {
    name: 'App'
  };
</script>