<template>
    <main class="columns ">
      <div class="column is-full ">
        <CabecalhoLogo />
      </div>
    </main>
    <div class="cadastrar-produto">
      <CadastrarProduto />
    </div> 
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import CabecalhoLogo from '../src/components/Cabecalho.vue'
import CadastrarProduto from '../src/components/CadastrarProduto.vue'
export default defineComponent({
  name: 'App',
  components: {
    CabecalhoLogo,
    CadastrarProduto
  }
});
</script>

<style scoped>
</style>

