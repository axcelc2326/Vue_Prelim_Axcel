<script>
import ProductItem from './Item.vue'
export default {

    name: 'ProductList',
    props: ['products'],
    components: {ProductItem},
    data(){
        return{

        }
    },
    methods: {
      
    }
}

</script>

<template>
  <div class="product-list">
        <h2>Product List</h2>
        <div class="list-container">
          <ProductItem v-for="product in products" :key="product.id" :product="product" />
        </div>       
  </div>
</template>

<style>
    .product-list{
      background-color: black;
      width: 300px;
      border: 2px solid red;
      text-align: center;
      color: white;
      padding: 5px;

    }
</style>