<template>
  <v-btn
    @click="() => vetor.push({nome: 'teste', idade:2})"
  >
    clique para adicionar
  </v-btn>
  <v-row>
    <v-col>
      <v-card
        v-for="(pessoa, i) in vetor"
        :key="i"
        class="ma-5"
        :title="pessoa.nome"
        :subtitle="pessoa.idade"
      >

      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'funcoesPage',
  data () {
    return {
      vetor: [
        {
          nome: 'Bernardo',
          idade: 19
        },
        {
          nome: 'oi',
          idade: 1
        },
        {
          nome: 'dasd',
          idade: 18
        },
        {
          nome: 'kdjohadioksla',
          idade: 20
        },
        {
          nome: 'djaiuhgdh',
          idade: 99
        },
      ],
      dois: 2,
    }
  }
}
</script>

<style>

</style>
