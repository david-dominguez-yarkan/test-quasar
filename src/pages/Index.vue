<template>
  <q-page class="flex flex-center">
    <q-form class="q-gutter-md">
      <q-input
        v-model="text1"
        label="text1"
        :rules="[
          (val) => !!val || 'This field is required',
          (val) => !falgs.flag1 || 'The flag1 must be activaed'
        ]"
      >
      </q-input>
      <q-input
        v-model="text2"
        label="text2"
        :rules="[(val) => !!val || 'This field is required']"
      >
      </q-input>
    </q-form>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data() {
    return {
      text1: '',
      text2: '',
      flags: {
        flag1: false,
        flag2: false
      }
    }
  }
}
</script>
