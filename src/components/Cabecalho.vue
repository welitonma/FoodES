<template>
    <div class="container-fluid p-0 m-0 bg-dark ">
        <div class="row">
            <div class="titulo col-6 d-flex justify-content-end py-5">
                FastFome
            </div>
            <div class="col-6 d-flex py-4">
                <img src="../assets/logo.png" alt="">
            </div>
        </div>
    </div>
    <nav class="navbar navbar-expand bg-dark">
        <div class="container">
            <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
                <ul class="navbar-nav">
                    <li class="nav-item active">
                        <a class="nav-link text-white text-decoration-none" href="#">Inicio</a>
                    </li>
                    <li class="nav-item ">
                        <a class="nav-link text-white text-decoration-none" href="#">Cadastrar</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-white text-decoration-none" href="./Cardapio.vue">Cardápio</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script lang="ts">

import { defineComponent } from 'vue';

export default defineComponent({
    name: 'CabecalhoLogo'
})

</script>

<style scoped>

.navbar-nav .nav-item:hover {
    background-color: #b9913b;
  }
img {
    padding: 1%;
    width: 150px;
    height: 100px;
}
.titulo {
    color: rgb(224, 228, 18);
    font-size: 50px;
    font-family: Georgia, 'Times New Roman', Times, serif;
}
</style>