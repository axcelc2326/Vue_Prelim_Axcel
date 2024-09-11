<script>
export default {
    
    name: 'ProductItem',
    props: ['product'],
    components: ['product'],
    methods: {
        addToCart(product){
            console.log(product)
        }
    }
}
</script>

<template>
  <div class="item">
    <h3>{{ product.name }}</h3>
    <p>Price: {{ product.price }}</p>
    <button @click="addToCart(product)">Add to Cart</button>
  </div>
</template>

<style>
    .item{
      background-color: #333;
      width: 100px;
      border: 2px solid white;
      text-align: center;
      color: white;
      padding: 5px;
    }
</style>