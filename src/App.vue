<script>
import ProductItem from './components/Item.vue';
import AddCart from './components/ItemList.vue';

export default{
  name: 'App',
  components: {AddCart, ProductItem},
  data(){
    return{
      products: [
        {id: 1, name: 'Product 1', price: 10, isVisible: true},
        {id: 2, name: 'Product 2', price: 20, isVisible: true},
        {id: 3, name: 'Product 3', price: 30, isVisible: false},
        {id: 4, name: 'Product 4', price: 40, isVisible: false},
        {id: 5, name: 'Product 5', price: 50, isVisible: false},
        {id: 6, name: 'Product 6', price: 60, isVisible: false},
        {id: 7, name: 'Product 7', price: 70, isVisible: true},
        {id: 8, name: 'Product 8', price: 80, isVisible: true},
        {id: 9, name: 'Product 9', price: 90, isVisible: true}
      ],
    }
  }
}
</script>

<template>
  <ForTop/>
  <AddCart :products="products"/>  
</template>

<style scoped>
  
</style>