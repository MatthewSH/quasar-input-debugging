<template>
  <q-page class="flex flex-center">
    <q-card>
      <q-input filled dense label="Number" inputmode="numeric" class="q-mb-md" v-model="num"/>
      <q-input filled dense label="Date" type="date" class="q-mb-md" v-model="date"/>
      <q-input filled dense label="Time" type="time" v-model="time"/>
    </q-card>
  </q-page>
</template>

<script>
import { defineComponent, ref} from 'vue';

export default defineComponent({
  name: 'PageIndex',
  setup() {
    return { num: ref(null), date: ref(null), time: ref(null)}
  }
})
</script>
