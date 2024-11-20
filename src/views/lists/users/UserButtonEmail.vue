<template>
  <div>
    <SuperTable
      @click.stop
      :showMap="true"
      :model="model"
      :displayMapField="false"
      :parentKeyValuePair="{
        parentFKey: 'recipient_id',
        parentFVal: +item.id,
        parentItem: item,
      }"
      justCreateButton
      createButtonText="Mail"
    />
    <!--:fetchFlags="fetchFlags"-->
  </div>
</template>

<script>
import { SuperTable } from 'wizweb-fe'
import Mail from 'src/models/orm-api/Mail'
export default {
  name: "EventButtonAttend",
  components: {
    SuperTable,
  },
  data() {
    return {
      model: Mail
    }
  },
  props: {
    item: {
      type: Object,
      default: () => {
      }
    },
    superOptions: {
      type: Object,
      default: () => {
      }
    },
  }
}
</script>

<style scoped>

</style>
