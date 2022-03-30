<template>
  <header class="container m-3 card shadow-sm mx-auto">
        <div class="container">
            <div class="row">
                <p> id=$product["id"]</p>
                <!-- 相片 -->
                <div class="col-md-4 p-3 d-flex align-items-center">
                    <img class="card-img-top d-block mx-auto" src="">
                </div>
                <!-- 相片 -->

                <!-- 商品內容 -->
                <div class="col-md-8 ">

                    <!-- 商品資訊 -->
                    <div class="mt-3">
                        <h1 class="fs-1 fw-bolder">
                            $product["name"]
                        </h1>

                        <div class="fs-6">
                            <p class="text-decoration-line-through"> 原價 $
                                $product["o-price"]
                            </p>
                            <p class="fs-5 text-danger fw-bolder">優惠價$
                                $product["price"]
                            </p>
                        </div>

                    </div>
                    <!-- 商品資訊 -->

                    <!-- 訂購按鈕 -->
                    <label class="small fw-bolder pt-5">購買數量</label>

                    <div>
                        <div class="input-group" role="group" aria-label="Basic mixed styles example">
                            <button id="min" class="btn border-danger text-danger col-1" type="button" value="-">-
                            </button>
                            <input id="num" name="num" class="btn border-danger text-dark col-2 " type="text" value="1"
                                readonly>
                            <buttont id="add" class="btn border-danger text-danger col-1" value="+">+
                            </buttont>
                            <label class="px-3 d-flex align-items-bottom"><small>庫存數量：$product["qty"]</small>
                            </label>
                        </div>
                        <input type="submit" class="btn btn-danger mt-3 add-btn">加入購物車</input>
                    </div>

                    </p>
                    <p id="message" class="text-success"></p>

                </div>
                <!-- 訂購按鈕 -->

            </div>
            <!-- 商品內容 -->

        </div>
        </div>
    </header>

    <section>
        <div class="container card shadow-sm p-3">
            <hr>
            <div class="container pt-2 pb-5">
                <h2 class="fs-3 fw-bolder text-danger">商品詳細介紹</h2>
                <div class="align-items-center justify-content-center ">
                    <?= $product["desc"] ?>
                </div>
            </div>
        </div>
    </section>
</template>