<template>
    <div>
        <h2>about</h2>
        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
        <p>api response:</p>
        <div>{{ data }}</div>
    </div>
</template>

<script setup>
   const { data } = await useFetch('/api/currency/GBP')
</script>

<style scoped>
h2{
    margin-bottom: 20px;
    font-size: 30px;
}

p{
    margin: 20px 0;
}
</style>