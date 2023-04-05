<script setup>
    import './style.scss'

    const props = defineProps({
        img: String,
        amount: Number,
        price: Number
    })

</script>

<template>
    <div class="product">
        <div class="product__img">
            <img :src="props.img">
        </div>
        <div class="product__info">
            <p class="info__title">Коробка</p>
            <p class="info__title">Количество: {{ props.amount }} шт.</p>
            <p class="info__title">Цена: {{ props.price }} руб.</p>
        </div>
        <button class="product__add-to-cart">Добавить в корзину</button>
    </div>
</template>