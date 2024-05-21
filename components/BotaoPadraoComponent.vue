<template>
  <v-btn
    :text="text"
    :color="color? color: '#fff'"
    @click="emitirEvento()"
  ></v-btn>
</template>

<script>
export default {
  name: 'BotaoPadraoComponent',
  data() {
    return {

    };
  },

  props: {
    text: {
      type: String
    },
    color: {
      type: String,
    },
  },

  methods: {
    emitirEvento() {
      this.$emit('clicouBotao', 2);
    }
  },
}
</script>
