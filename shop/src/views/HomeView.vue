<template>
  <div class="home">
    <!-- 商品區 -->
    <section class="p-1 col-md-9 col-sm-2 shadow-sm card-group">
      <div class="p-1">
        <div>
          <h2 class="p-2">活動商品</h2>
        </div>
        <div class="row row-cols-2 row-cols-lg-4 row-cols-sm-2 ">
          <template v-for="product in products" :key="product">
            <ProductCard v-bind="product" />
          </template>
        </div>
      </div>


    </section>
    <!-- 商品區 -->
  </div>
</template>

<script>
// @ is an alias to /src
import ProductCard from '@/components/ProductCard.vue'

export default {
  name: 'HomeView',
  components: {
    ProductCard
  }
}
</script>
