<template>
  <q-page class="flex flex-center">
    <q-input v-model="value" />
  </q-page>
</template>
<script>
export default {
  name: 'PageIndex',
  data() {
    return {
      value: 'This is text'
    }
  }
}
</script>
