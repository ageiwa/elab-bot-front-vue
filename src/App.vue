<script setup>
    import Product from '/src/components/Product/Product.vue'

    const products = [
        {
            img: '/public/box1.jpg',
            amount: 1,
            price: 250
        },
        {
            img: '/public/box2.jpg',
            amount: 2,
            price: 350
        },
        {
            img: '/public/box3.jpg',
            amount: 3,
            price: 450
        },
    ]
</script>

<template>
    <div class="container">
        <Product v-for="product in products"
            :img="product.img"
            :amount="product.amount"
            :price="product.price"
        />
    </div>
</template>