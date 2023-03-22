<!-- Copyright(c) 2023, Carlos Astengo, All Rights Reserved -->
<script setup>
    defineProps({
    title: {
        type: String,
        required: true
    }
    })
</script>

<template>
    <div class="H-Stack">
        <img src="..\assets\Images\ProgrammerArtLogo.png" alt="Logo" width="80" height="80">
        <div class="TextArea">
            <h1 class="teamName">{{ title }}</h1>
            <h5>
            Breaking Source Tree since 2023
            </h5>
        </div>
    </div>
</template>

<style scoped>
    .H-Stack
    {
        display: flex;
    }

    h1 
    {
    font-weight: 500;
    font-size: 2.6rem;
    top: -10px;
    }

    h3 
    {
    font-size: 1.2rem;
    }

    .TextArea h1,
    .TextArea h5 
    {
        padding-left: 20px;
    }

    .TextArea h5 
    {
        color: whitesmoke;
    }
</style>
