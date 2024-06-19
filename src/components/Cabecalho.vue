<script setup>
defineProps({
  titulo: {
    type: String,
    required: true
  },
  logo: {
        type: String,
        required: true
    }
})
</script>

<template>
    <nav>
        <div id="cab">
            <div id="div_logo">
                <span>
                    <img :src="logo" >
                </span>
            </div>
            <div id="div_titulo">
                <span>{{ titulo }}</span>
            </div>
        </div>
    </nav>
</template>

<style scoped>
    nav {
        background-color: white;
        color: white;
        padding: 10px;
        right: 0px;
        width: 100%;
        position: absolute;
        top: 0px;
    }
    #cab{
        display: flex;
        justify-content: space-between;
    }
    #div_logo{
        display: flex;
        align-items: center;
        margin: auto;
    }
</style>