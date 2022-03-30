<template>
    <div class="container p-3 ">
        <div class="card p-3">
            <h1>訂單詳情</h1>
            <table class="table-info table-bordered text-center">
                <thead>
                    <td>商品圖片</td>
                    <td>商品名稱</td>
                    <td>單價</td>
                    <td>數量</td>
                    <td>小計</td>
                    <td>操作</td>
                </thead>
                <tbody>
                    <tr>
                        <td><img src="" class="d-block" style="width: 8rem;"></td>
                        <td>{{name}}</td>
                        <td class="text-end">${{price}}</td>
                        <td class="text-end">x{{value}}</td>
                        <!-- <?php
                                $subtotal = $row["price"] * $value;
                                $total += $subtotal;
                                ?> -->
                        <td class="text-end">${{subtotal}}</td>
                        <td>
                            <a href="商品頁面" class="btn btn-info">詳細</a>
                            <a href="刪除api" class="btn btn-danger">刪除</a>
                        </td>
                    </tr>

                    <!-- <?php
                        endforeach;
                    endif; //Cart 存在
                    ?> -->
                </tbody>
                <tfoot>
                    <tr>
                        <td class="text-end" colspan="5">總價: ${{total}}</td>
                    </tr>
                </tfoot>

            </table>

            <div class="container">
                <div class="pt-3 mx-auto align-items-center">
                    <div>
                        <h2 class="pt-5">收件資訊</h2>
                        <p>請在下列表單輸入您的收件資訊</p>
                    </div>

                    <form action="#" method="post">

                        <div class="row mb-3 pt-3">
                            <label for="inputname" class="text-right col-sm-3 col-form-label">收件人姓名</label>
                            <div class="col-sm-9">
                                <input type="text" class="form-control" id="inputname">


                            </div>
                        </div>

                        <div class="row mb-3">
                            <label for="inputEmail3" class="text-right col-sm-3 col-form-label">手機號碼</label>
                            <div class="col-sm-9">
                                <input type="email" class="form-control" id="inputEmail3">
                            </div>
                        </div>

                        <div class="row mb-3 pt-3">
                            <label for="input_id" class="text-right col-sm-3 col-form-label">連絡電話</label>
                            <div class="col-sm-9">
                                <input type="text" class="form-control" id="input_id">
                            </div>
                        </div>

                        <div class="row mb-3 pt-3">
                            <label for="input_addres" class="text-right col-sm-3 col-form-label">收件地址</label>

                            <div class="col-sm-9">

                                <input type="text" class="form-control" id="input_addres">
                            </div>
                        </div>

                        <div class="row mb-3 pt-3">
                            <label for="input_addres" class="text-right col-sm-3 col-form-label">備註欄位</label>
                            <div class="col-sm-9">
                                <input type="text" class="form-control" id="input_addres">
                            </div>
                        </div>

                        <div class="row mb-3 p-3">
                            <p>請選擇取貨方式</p>
                            <div class="form-check">
                                <input class="form-check-input" type="radio" name="flexRadioDefault" id="711">
                                <label class="form-check-label" for="flexRadioDefault1">
                                    7-11超商店到店
                                </label>
                            </div>
                            <div class="form-check">
                                <input class="form-check-input" type="radio" name="flexRadioDefault" id="711">
                                <label class="form-check-label" for="flexRadioDefault1">
                                    全家便利商店
                                </label>
                            </div>
                            <div class="form-check">
                                <input class="form-check-input" type="radio" name="flexRadioDefault" id="711">
                                <label class="form-check-label" for="flexRadioDefault1">
                                    OK便利商店
                                </label>
                            </div>
                            <div class="form-check">
                                <input class="form-check-input" type="radio" name="flexRadioDefault" id="711">
                                <label class="form-check-label" for="flexRadioDefault1">
                                    宅配
                                </label>
                            </div>
                        </div>
                    </form>
                </div>
            </div>


            <div class="d-flex justify-content-end pt-3">
                <a type="button" class=" btn btn-danger" href="結帳(清空php)">結帳</a>
            </div>

        </div>
    </div>
</template>


