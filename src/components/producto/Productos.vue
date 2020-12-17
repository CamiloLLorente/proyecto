<template>
  <div class="wrapper">
    <Header />
    <div class="contenedor">
      <div v-if="porductoAction == 'home'">
        <Card />
        <!-- <CardTable /> -->
      </div>
      <div v-if="porductoAction == 'editar'">
        <!-- <EditarProducto /> -->
      </div>
      <div v-if="porductoAction == 'agregar'">
        <!-- <AgregarProducto /> -->
      </div>
      <div v-if="porductoAction == 'nuevo'">
        <Card />
        <!-- <CardTable /> -->
      </div>
      
    </div>
    
  </div>
</template>

<script>
import Header from '@/components/Header'
import Card from '@/components/producto/Card'
// import AgregarProducto from '@/components/producto/AgregarProducto'
/*import EditarProducto from '@/components/producto/EditarProducto'

import CardTable from '@/components/producto/CardTable' */
import { mapState } from 'vuex'
export default {
  
  name: "Productos",
  data(){
    return{
      codigo:''
    }
  },

  components:{
    Header,
    Card,
    // AgregarProducto
   /* CardTable,
    EditarProducto,
    */

  
  },
  computed:{
    ...mapState(['porductoAction'])
  }
  
};
</script>

<style  scoped>
  .contenedor{
    padding: 15px 10px;

  }
</style>
