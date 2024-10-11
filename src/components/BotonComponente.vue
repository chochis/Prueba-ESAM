<template>
    <button class="boton-componente">
    <div class="content-wrapper">
        <i :class="['mdi v-icon notranslate v-theme--light', iconClass]" class="icono"></i>
        <h3 class="titulo">{{ title }}</h3>
    </div>
    </button>
</template>

<script>
export default {
    name: 'BotonComponente',
    props: {
    title: {
        type: String,
        required: true
    },
    iconClass: {
        type: String,
        required: true
    }
    }
}
</script>

<style scoped>
.boton-componente {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    background-color: #f0f0f0;
    border: none;
    border-radius: 8px;
    padding: 20px;
    width: 100%;
    height: 150px;
    cursor: pointer;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    transition: background-color 0.3s ease;
}

.boton-componente:hover {
    background-color: #554fa1;
}

.content-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.icono {
    font-size: 50px;
    margin-bottom: 10px;
}

.titulo {
    font-size: 16px;
    text-align: center;
    margin: 0;
    font-weight: bold;
    color: #333;
}
</style>