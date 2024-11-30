<script setup lang="ts">
const props = defineProps({
    text: String,
    id: String
})
</script>

<template>
    <input 
        class="custom-checkbox"
        :id="props.id" 
        type="checkbox">
        <label :for="props.id">
        {{ props.text }}
    </label>
</template>

<style lang="scss">
    @import "./assets/scss/components/UI/_Checkbox.scss";
    @import "./assets/scss/base/_utilities.scss";

</style>

<!--  -->