<script setup>
    import { useCounterStore } from '../stores/counter.js'
    import CartIcon from './icons/CartIcon.vue'

    const store = useCounterStore()

    // const{ count } = storeToRefs(store)
</script>

<template>
    <div class="container">
        <CartIcon class="cart-icosn"></CartIcon>
        <span>{{store.count}}</span>
    </div>
</template>

<style>
    .container{
        position: relative;
    }
    span{
        width: 17px;
        height: 17px;
        background-color: var(--delete-color);
        color: white;
        border-radius: 50%;
        

        position: absolute;
        right: -0.5rem;
        top: 50%;
        text-align: center;
    }
</style>