<template>
    <div>
        <div v-for="p in products" :key="p.id">
            <ProductCard :product="p"/>
        </div>

    </div>
</template>
<script setup>


const {  data: products } = await useFetch('https://fakestoreapi.com/products')
   
  
</script>
<style  scoped>

</style>