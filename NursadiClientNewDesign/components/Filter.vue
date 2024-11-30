<script setup lang="ts">
import Checkbox from './UI/Checkbox.vue';
import InputText from './UI/InputText.vue';
const props = defineProps({
    title: String
})
</script>

<template>
    <div class="filter ff-regular">
        <h2 class="zagolovok mb-2">Фильтры</h2>
        <div class="zagolovok filter-title mb-3 b">
            <h3>{{ props.title }}</h3>
        </div>
        <div class="check1">
            <Checkbox :id="'ch1'" :text="'Алматы'"></Checkbox>
        </div>
        <div class="check2 mt-1">
            <Checkbox :id="'ch2'" :text="'Нур-Султан'"></Checkbox>
        </div>
        <div class="check3 mt-1">
            <Checkbox :id="'ch3'" :text="'Караганда'"></Checkbox>
        </div>
        <div class="check4 mt-1">
            <Checkbox :id="'ch4'" :text="'Шымкент'"></Checkbox>
        </div>
        <div class="check5 mt-1">
            <Checkbox :id="'ch5'" :text="'Атырау'"></Checkbox>
        </div>
        <div class="check6 mt-1">
            <Checkbox :id="'ch6'" :text="'Тараз'"></Checkbox>
        </div>
        <div class="check7 mt-1">
            <Checkbox :id="'ch7'" :text="'Кокшетау'"></Checkbox>
        </div>
        <h3 class="mb-1 mt-2 b">Средняя цена</h3>
        <div class="filter-price mb-2">
            <label class="me-2">От</label>
            <InputText></InputText>
            <label class="ms-2 me-2">До</label>
            <InputText></InputText>
        </div>
        
        <div class="d-flex">
            <label class="switch">
                <input id="ch" type="checkbox">
                <span class="slider round"></span>
            </label>
            <label class="ms-1">Только от проверенных</label>
        </div>
       
        <div class="filter__buttons mt-3">
            <button class="btn mb-1">Применить</button>
            <button class="btn">Сбросить фильтры</button>
        </div>
    </div>
</template>

<style lang="scss">

  @import "./assets/scss/components/_Filter.scss"; 
  @import "./assets/scss/base/_utilities.scss";
  @import "./assets/scss/base/mainPage.scss"
</style>