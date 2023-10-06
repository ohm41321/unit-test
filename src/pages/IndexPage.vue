<!-- <template>
  <q-page class="flex flex-center">
    <img
      alt="Quasar logo"
      src="~assets/quasar-logo-vertical.svg"
      style="width: 200px; height: 200px"
    >
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage'
})
</script> -->



<!-- IndexPage.vue -->
<template>
  <div class="htmlClass">
    <h1>{{ title }}</h1>
    <InputPage/>
    <FunctionPage/>
  </div>
</template>


<script>
import InputPage from '../pages/InputPage.vue'
import FunctionPage from '../pages/FunctionPage.vue'

export default {
  name: 'HtmlComponent',
  components:{InputPage, FunctionPage},
  data() {
    return {
      title: 'Athit Fongkhaimuk',
    }
  },
}
</script>

<style scoped></style>