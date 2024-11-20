<template>
  <q-btn @click.stop="handleClick" flat primary>
    Mail
  </q-btn>
</template>

<script>

export default {
  name: "EventButtonAttend",
  components: {
  },
  data(){
    return {
    }
  },
  props: {
    item: {
      type: Object,
      default: () => {}
    },
    superOptions: {
      type: Object,
      default: () => {}
    },
  },
  methods: {
    handleClick(){
      console.log(122)
    },
  }
}
</script>

<style scoped>

</style>
