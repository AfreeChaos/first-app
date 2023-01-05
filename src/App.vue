<template>
  <header class="header px-1">
    <a href="#" class="nav">AllProducts</a>
    <a href="#" class="nav">Smartphones</a>
    <a href="#" class="nav">Notebooks</a>
    <button class="button-cart">Cart</button>
  </header>
  <section class="products container">
    <div>
      <img src="./assets/item.jpeg" alt="" class="img">
      <h3 class="h3">{{ item.name }}</h3>
      <p>{{ item.price }}€</p>
      <button class="button-add">Add to cart</button>
    </div>
    <div></div>
    <div></div>
  </section>
</template>

<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
</script>



<style scoped>
.header {
  background: #444;
  padding: 20px;
  display: flex;
  justify-content: center;
  align-content: center;
}
.nav {
  color: #fff;
  margin-left: 36px;  
  margin-right: 36px;
}
.button-cart {
  color: #fff;
  padding: 4px 24px 4px 24px;
  margin-left: 112px;
  background: #5454fe;
  border-radius: 4px;
}
.products {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  margin: auto;
  margin-top: 64px;
  gap: 24px;
}
.img {
  width: 100%;
}
.h3 {
  margin-top: 20px;
  font-size: 24px;
  line-height: 32px;
}
.button-add {
  width: 100%;
  color: #fff;
  background: rgb(0, 130, 0);
  border-radius: 4px;
  padding: 24px 4px 0 0;
}
</style>
