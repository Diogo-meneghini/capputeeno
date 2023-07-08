<script setup>
    import Input from './Input.vue'
    import ShoppingCart from './ShoppingCart.vue'
    // import AccountIcon from './icons/AccountIcon.vue'

</script>

<template>
    <header>
        <div class="logo">
            <a href="/home">Capputeeno</a>
        </div>
        <div class="container">
            <Input></Input>
            <a href="/cart">
                <ShoppingCart class="cart"></ShoppingCart>
            </a>
            <a href="/account">
                <ion-icon name="person"></ion-icon>
            </a>
        </div>
    </header>
</template>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&family=Saira+Stencil+One&display=swap');
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 144rem;
        /* width: 100vw; */
        height: 8rem;
        flex-shrink: 0;
    }
    .logo a{
        font-style: normal;
        font-weight: 400;
        line-height: 150%;
        font-size: 4rem;
        color: var(--logo-color);
        font-family: 'Saira Stencil One';
        cursor: pointer;
        text-decoration: none;
        

        display: flex;
        width: 54.4rem;
        height: 8rem;
        flex-direction: column;
        justify-content: center;
        flex-shrink: 0;
        padding-left: 16rem;
    }
    .container{
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 2.4rem;
    }
    .cart{
        align-items: center;
    }
    ion-icon{
        font-size: 2.4rem;
        color: black;
        padding-top: 0.7rem;
    }
</style>