<script setup lang="ts">

</script>

<template>
    <div class="short-product-card__container">
        <div class="d-flex">
            <img src="/img/beton.jpg" class="mt-1 short-product-card__img ma">
        </div>
        <div class="wrap">
            <div class="short-product-card__wrapper-text">
            <h3 class="ff-regular short-product-card__title">БЕТОН ДОРОЖНЫЙ КЛАССА В5 ГОСТ 7473-2010</h3>
            <h6 class="short-product-card__description">Бетон высокой прочности, термоустойчевый.</h6>
        </div>
        <div class="ff-regular short-product-card__wrapper-price">
            <div class="short-product-card__price">
                <label for="">2 833.33₸</label>
                <label class="ms-1 des-item">Сред. розн. цена</label>
            </div>
            <div class="short-product-card__priceOpt">
                <label for="">2 833.33₸</label>
                <label class="ms-1 des-item">Сред. опт. цена</label>
            </div>
            <div class="short-product-card__postav">
                <label for="">14</label>
                <label class="ms-1 des-item" for="">Поставщиков</label>
            </div>
            <div class="d-flex mt-1">
                <button class="short-product-card__btn btn ff-regular">
                <i class="fa fa-shopping-cart me-1" aria-hidden="true"></i>В корзину</button>
            </div>
            
        </div>
        </div>
        
    </div>
</template>

<style lang="scss" scoped>
    @import "./assets/scss/components/Product/_ShortProductCard.scss";
    @import "./assets/scss/base/_utilities.scss";
</style>