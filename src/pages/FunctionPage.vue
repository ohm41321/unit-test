
<template>
  <div class="htmlClass">
    <h1>{{ title }}</h1>
    <form>
      <input type="text" id="firstValue" v-model="firstValue" />
      <input type="text" id="secondValue" v-model="secondValue" />
      <input type="text" id="answerValue" v-model="answerValue" />
      <button @click="addition(firstValue,secondValue)" >Addition</button>
      <button @click="subtraction(firstValue,secondValue)" >Subtraction</button>
      <button @click="multiplication(firstValue,secondValue)" >Multiplication</button>
      <button @click="divide(firstValue,secondValue)" >Divide</button>
  </form>
  </div>
</template>
<script>

export default {
  name: 'HtmlComponent',
  data() {
    return {
      title: 'Athit Fongkhaimuk',
      firstValue:0,
      secondValue:0,
      answerValue:0
    }
  },
  methods: {
    // https://jestjs.io/docs/using-matchers
    // https://www.philbarresi.com/jest-test-guide/
    addition(first, second) {
      this.answerValue =  Number(first) + Number(second)
      return this.answerValue;
    },
    subtraction(first, second ) {
      this.answerValue =  Number(first) - Number(second)
      return this.answerValue;
    },
    multiplication(first, second ) {
      this.answerValue =  Number(first) * Number(second)
      return this.answerValue;
    },
    divide(first, second) {
      this.answerValue =  Number(first) / Number(second)
      return this.answerValue;
    },
  },
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
