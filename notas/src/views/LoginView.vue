<template>
  <div class="row">
    <h1>Bem vindo</h1>
    <h4>É novo por aqui? Crie uma conta</h4>

    <form @submit.prevent="login" class="">
      <div style="display:flex; flex-direction:column">
        <label for="email"><strong>Email</strong></label>
        <input type="text" id="email" v-model="email" required placeholder="Digite o seu email">
      </div>

      <div class="col-6">
        <label for="passwaord"><strong>Senha</strong></label>
        <input type="text" id="passwaord" v-model="email" required placeholder="Digite a sua senha">
      </div>

      <div>
        <button type="submit">Entrar</button>
      </div>
    </form>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'
export default defineComponent({
  data () {
    return {
      username: '',
      password: ''
    }
  },
  methods: {
    login () {
      console.log('entrou')
    }
  }
})
</script>

<style>

*,
*::after,
*::before{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
}

.row-login{
  margin-left: 0;
}

.left-login{
  background-color: #f2f2f2;
}
</style>
