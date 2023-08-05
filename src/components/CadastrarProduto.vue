<template>
    <header class="text-center">
        <h1 class="titulo-cadastro">
            CADASTRAR LANCHE
        </h1>
    </header>
    <form @submit.prevent="handleSubmit">
        <div class="col-md-4 mx-auto py-5">
            <label for="nomeLanche">Nome Produto</label>
            <input type="text" class="nomeLanche form-control" aria-label="First name" v-model="nomeProduto" required>

            <label for="tipoDeCarne">Tipo de carne</label>
            <select class="tipoDeCarne form-select form-select-md mb-3" aria-label=".form-select-md example" v-model="tipoDeCarne">
                <option selected>Escolher</option>
                <option value="1">Tradicional</option>
                <option value="2">Picanha</option>
                <option value="3">Gourmet</option>
            </select>

            <label for="quantidadeCarne">Quantidade de carne</label>
            <input type="number" class="quantidadeCarne form-control" aria-label="Last name" v-model="quantidadeDeCarne">

            <label for="nomeProduto">Quantidade de ovo</label>
            <input type="number" class="quantidadeDeOvo form-control" aria-label="First name" v-model="quantidadeDeOvo">

            <label for="tipoDeQueijo">Tipo de queijo</label>
            <select class="tipoDeQueijo form-select form-select-md mb-3" aria-label=".form-select-md example" v-model="tipoDeQueijo">
                <option selected>Escolher</option>
                <option value="1">Mussarela</option>
                <option value="2">Cheedar</option>
            </select>

            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="flexCheckChecked" v-model="selecionarBacon">
                <label class="form-check-label" for="flexCheckChecked">
                    Bacon
                </label>
            </div>
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="flexCheckChecked" v-model="selecionarPresunto">
                <label class="form-check-label" for="flexCheckChecked">
                    Presunto
                </label>
            </div>
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="flexCheckChecked" v-model="selecionarAlface">
                <label class="form-check-label" for="flexCheckChecked">
                    Alface
                </label>
            </div>
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="flexCheckChecked" v-model="selecionarTomate">
                <label class="form-check-label" for="flexCheckChecked">
                    Tomate
                </label>
            </div>
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="flexCheckChecked" v-model="selecionarBatataPalha">
                <label class="form-check-label" for="flexCheckChecked">
                    Batata Palha
                </label>
            </div>
            <div class="d-flex justify-content-end">
                <button type="submit">Cadastrar</button>
            </div>
        </div>
    </form>
    <footer class="text-center bg-dark py-3">
        <h1 class="assinatura">Desenvolvido por Deivid Ferreira</h1>
    </footer>
</template>

<script setup lang="ts">

import { ref } from 'vue';

const nomeProduto = ref('');
const tipoDeCarne = ref('');
const quantidadeDeCarne = ref(0);
const quantidadeDeOvo = ref(0);
const tipoDeQueijo = ref('');
const selecionarAlface = ref(false);
const selecionarBacon = ref(false);
const selecionarBatataPalha = ref(false);
const selecionarPresunto = ref(false);
const selecionarTomate = ref(false);

const handleSubmit = () => {
    console.log("Nome", nomeProduto.value),
    console.log("QtdCarne", quantidadeDeCarne.value),
    console.log("Tem Alface", selecionarAlface.value)
}

</script>

<style scoped>
form {
    font-family: Georgia, 'Times New Roman', Times, serif;
}

.titulo-cadastro {
    font-family: Georgia, 'Times New Roman', Times, serif;
}

footer {
    color: white;
}

.assinatura {
    font-size: 20px;
}
</style>



