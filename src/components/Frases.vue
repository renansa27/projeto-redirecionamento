<template>
  <div class="div">
    <span class="texto">{{msg}}</span>
  </div>
</template>

<script>
export default {
  data() {
    return {
      frases: [
        { value: "Quanto mais agradecemos, mais coisas boas acontecem." },
        { value: "Se você cansar, aprenda a descansar e não a desistir." },
        { value: "Quando você deseja o bem, o bem te deseja também." },
        { value: "A gratidão é a memória do coração." },
        { value: "Se você está cansado de recomeçar pare de desistir." },
        { value: "Seja você mesmo, todos os outros já existem." },
        { value: "Não coloque limite em seus sonhos, coloque fé." },
        { value: "Insista, persista e nunca desista." },
        { value: "Não existe caminho novo, existe um novo jeito de caminhar." },
        { value: "Passado é lição para refletir, não para repetir." },
        { value: "Amar o que faz e ser feliz no caminho." },
        { value: "Coisas pequenas tornam-se grandes quando feitas com amor." },
        { value: "Sucesso é uma questão de decisão." },
        { value: "Faça valer a pena, as oportunidades não voltam." }
      ],
      msg: null
    };
  },
  methods: {
    getFrase() {
      var num = Math.floor(Math.random() * (13 - 0)) + 0;
      this.msg = this.frases[num].value;
    }
  },
  mounted() {
    this.getFrase();
  }
};
</script>

<style>
.div {
  text-align: center;
  text-justify: center;
  border: 1px solid black;
  border-radius: 3px;
  height: 30;
  width: 170px;
  font-size: 16px;
  font-family: cursive;
  font-style: italic;
  font-weight: bold;
}
</style>