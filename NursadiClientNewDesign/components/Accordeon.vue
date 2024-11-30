<script setup>
import Checkbox from './UI/Checkbox.vue';

const props = defineProps({
    items:{
        Array,
    },
})

const list = ref(
    props.items.map((item) =>{
        return {...item,open:false};
    })
)


function openOrClose(item){
    item.open = !item.open;
    console.log(item.open);
}

</script>

<template>
    <div>
        <div v-for="(item,idx) in list" :key="idx">
            <h2>
                <button class="mainItem ff-primary" :class="{mainItemActive: item.open}" @click="openOrClose(item)">
                    <span>
                        {{ item.title }}
                    </span>
                    <Icon name="mdi:chevron-down"></Icon>
                </button>
            </h2>
            
            <div class="active" :class="{hidden: !item.open}">
                <div v-for="(i,index) in item.subTitle" :key="index">
                    <Checkbox :id="`ch1${index}`" :text="i"></Checkbox>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
  .active{
    display: block;
    max-width: 200px;
    overflow-wrap: break-word;
    font-family: sans-serif;
  }

  .hidden{
    display: none
  }

  .mainItem{
    border: none;
    background-color:var(--clr-bg);
    font-weight: bold;
    font-size: 20px;
    width: 240px;
    height: 72px;
    cursor: pointer;
    text-align: left;
  }

  .mainItemActive{
        border: none;
        background-color: var(--clr-bg);
        font-weight: bold;
        color:#005BD1;
        font-size: 20px;

    }

  @import "./assets/scss/base/_root.scss";
  @import "./assets/scss/base/_utilities.scss";
</style>