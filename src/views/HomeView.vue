<template>
  <div class="home">
    <!-- 商品區 -->
            <section class="p-1 col-md-9 col-sm-2 shadow-sm card-group">
                <div class="p-1">
                    <div>
                        <h2 class="p-2">活動商品</h2>
                    </div>
                    <div class="row row-cols-2 row-cols-lg-4 row-cols-sm-2 ">
                        <!-- <?php
                        if ($result->num_rows > 0) :
                            for ($i = 0; $i < $total_records; $i++) :
                                $row = mysqli_fetch_assoc($result); //將陣列以欄位名索引 
                        ?> -->
                        <ProductCard/>
                        <!-- <?php endfor;  ?> -->
                    </div>
                </div>
                <!-- <?php else : ?>
                <h3> 沒有商品 </h3>
                <?php endif; ?> -->

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
