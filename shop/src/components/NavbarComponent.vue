<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container-fluid">
            <router-link to="/">
                <img src="/src/assets/img/logo.svg" alt="" width="30" height="30">
            </router-link>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02"
                aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <router-link to="/">HOME</router-link>
                    </li>
                </ul>
                <div class="m-1">
                    <!-- 登入前顯示 -->
                    <a href="#" class="btn btn-danger mx-1">登入</a>
                    <a href="#" class="btn btn-danger mx-1">註冊</a>
                    <!-- 登入後顯示 -->
                    <router-link to="/cart" class="btn btn-danger mx-1">
                        <i class="bi bi-cart-fill"></i> 購物車({{ currentQuantity }})
                    </router-link>
                    <a href="#" class="btn btn-danger mx-1">登出</a>
                </div>
            </div>


        </div>
    </nav>
</template>