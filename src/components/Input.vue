<script setup>
    import SearchIcon from './icons/SearchIcon.vue'

</script>

<template>
    <div>
        <input type="text" placeholder="Procurando por algo específico?">
        <SearchIcon class="icon"></SearchIcon>
    </div>
</template>

<style scoped>
    div{
        position: relative;
        width: 35.2rem;
        height: 4.2rem;
    }
    div input{
        width: 35.2rem;
        border-radius: 0.8rem;
        padding: 1rem 1.6rem;
        border: none;
        
        background-color: var(--bg-secondary);

        font-family: 'Arial';
        font-style: normal;
        font-weight: 400;
        font-size: 1.4rem;
        line-height: 2.2rem;
        color: var(--text-dark);
        
    }
    .icon{
        position: absolute;
        right: 2rem;
        top: 50%;
        transform: translateY(-50%);
    }
    
</style>