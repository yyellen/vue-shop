<template>
  <div class="col py-1" @click="redirectProduct(id)">
    <a href="">
      <!-- <p>商品編號：{{id}}</p> -->
      <div class="card p-1 h-100 shadow-sm">
        <div class="ratio ratio-1x1">
          <img :src="parseImgPath(img_path)" class="card-img-top cover">
        </div>
        <h5 class="text-truncate p-1">{{name}}</h5>
        <h6 class="text-danger p-1">優惠價${{price}}</h6>
      </div>
    </a>
  </div>
</template>

<style>
  body {
        font-family: 'Noto Sans SC', sans-serif;
        background-color: #eee;
        color: #121212;
  }

  header {
        width: 70%;
        height: 100%;
  }

  section {
        background-color: #FFF;
  }

  a {
        color: #121212;
        text-decoration: none;

  }

  a:hover {
        color: #121212;
        text-decoration: none;

  }
</style>