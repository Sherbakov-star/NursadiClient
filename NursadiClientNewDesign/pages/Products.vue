<script setup lang="ts">
 import Catalogue from '../components/Catalogue.vue';
 import BreadCrumbs from '../components/BreadCrumbs.vue';
 import ShortProductCard from '../components/Product/ShortProductCard.vue';
 import Filter from '../components/Filter.vue';
</script>
<template>
<link rel="stylesheet" href="path/to/font-awesome/css/font-awesome.min.css">
    <div class="wrapper">
        <header class="header">
            <div class="header__container _container">
                <NuxtLink to="/" class="header__logo"><img src="/img/logo.png"></NuxtLink>
          
                <Catalogue></Catalogue>
                
                <div class="header__combobox">
                    <select>
                        <option value="A">Алматы</option>
                        <option value="B">Нур-Султан</option>
                        <option value="-">Актюбиснкая область</option>
                        <option value="-">Алматинская область</option>
                    </select>
                </div>
                <nav class="header__menu menu">
                        <ul class="menu__list">
                            <li class="menu__item">
                                <a href="" class="menu__link">Главная</a>
                            </li>
                            <li class="menu__item">
                                <a href="" class="menu__link">Сборники</a>
                            </li>
                            <li class="menu__item">
                                <a href="" class="menu__link">Закупки</a>
                            </li>
                            <li class="menu__item">
                                <a href="" class="menu__link">Информация</a>
                            </li>
                            <li class="menu__item">
                                <a href="" class="menu__link">Контакты</a>
                            </li>
                            <li class="menu__item">
                                <a href="" class="menu__link">Войти</a>
                            </li>
                            <li class="menu__item">
                                <a href="" class="menu__link">Регистрация</a>
                            </li>
                        </ul>
                </nav>
                <div class="header__cart">
                    <i style="font-size:20px;padding-top:2px;" class="fa fa-shopping-basket"></i>
                </div>
            </div>
        </header>
        <main class="main">
            <BreadCrumbs></BreadCrumbs>
            <div class="wrapper-products">
                <!-- <Filter class="ms-3" :title="'Поставщики из городов'"></Filter> -->
                <div class="products ms-3 mt-3">
                    <ShortProductCard class="prod mb-3"></ShortProductCard>
                    <ShortProductCard class="prod mb-3"></ShortProductCard>
                    <ShortProductCard class="prod mb-3"></ShortProductCard>
                </div>
            </div>
        </main>
        <footer class="footer">
            <div class="footer__area">
                <div class="container">
                    <div class="row">S
                        
                            <div class="footer__content">
                                <div class="footer__head">
                                    <div class="footer__head__logo">
                                        <h2>
                                            <span>SADI.KZ</span>
                                        </h2>
                                    </div>
                                    <p>Единая база данных актуальных цен в строительстве. Новая инновационная система проведения закупочных процедур.</p>
                                    <a class="textBlack_small" href="/agreement">Пользовательское соглашение</a>
                                </div>
                            </div>
                            <div class="footer__content">
                                <div class="footer__head">
                                    <h4>Для Поставщиков</h4>
                                    <a class="textBlack_small" target="_blank" href="https://drive.google.com/file/d/1izqoRTSbC6nfL6ZVDj6CEegQ5Xl5uq6h/view?usp=sharing">Презентация для Поставщиков</a>
                                    <a class="textBlack_small" target="_blank" href="https://drive.google.com/file/d/1cXDW9by0JbvHYgwwoyzOFJsMLSEov0no/view?usp=sharing">Руководство пользователя для Поставщиков</a>
                                </div>
                            </div>
                            <div class="footer__content">
                                <div class="footer__head">
                                    <h4>Для Закупщиков</h4>
                                    <a target="_blank" href="https://drive.google.com/file/d/1-tqFFdiN5vZG3yx1AHViFiGK_8SJb-XY/view?usp=sharing" class="textBlack_small">Презентация для Закупщиков</a>
                                    <a target="_blank" href="https://drive.google.com/file/d/1HwqE1g3Is3KEUD6-cqwLdl9rNhL10QWK/view?usp=sharing" class="textBlack_small">Руководство пользователя для Закупщиков</a>
                                </div>
                            </div>
                            <div class="footer__content">
                                <div class="footer__head">
                                    <h4>Контакты</h4>
                                    <div class="footer__contacts">
                                        <p>
                                            <span>Телефон:</span>
                                            <a class="textBlack_small" href="tel:+77086083103">+7 (708) 608 31 03</a>
                                        </p>
                                        <p>
                                            <span>Email:</span>
                                            <a class="textBlack_small" href="mailto:info@sadi.kz">info@sadi.kz</a>
                                        </p>
                                        <p>
                                            <span>Skype:</span>
                                            Kairat Maukebayev
                                        </p>
                                    </div>
                                </div>
                            </div>
                       
                    </div>
                    <div class="row">
                        <div class="footer__content">
                                <div class="footer__head">
                                    <h4>Для Инвесторов</h4>
                                    <a target="_blank" href="https://drive.google.com/file/d/1YeV79TNPFQ_1ZedNwUIQfKLJHbxuK5Uh/view?usp=share_link" class="textBlack_small">Ищем частных инвесторов партнеров на развитие проекта</a>
                                </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="footer-area-bottom">
               <div class="container">
                    <div class="row">
                        <div class="copyright">
                            <p>
                                © Copyright 
                                <strong>TOO NurSADI</strong>
                                . All Rights Reserved
                            </p>
                        </div>
                    </div>
               </div>
            </div>
        </footer>
    </div>
</template>

<style lang="scss" scoped>
  @import "./assets/scss/base/mainPage.scss"; 
  @import 'https://pro.fontawesome.com/releases/v5.10.0/css/all.css';
  @import "./assets/scss/base/_utilities.scss";

</style>