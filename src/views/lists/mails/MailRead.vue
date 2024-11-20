<template>
    <SuperRecord
        :model="superRecordModel"
        :id="+$route.params.rId"
        :displayMapField="true"
        @initialLoadHappened="$emit('initialLoadHappened')"
    >
    </SuperRecord>
</template>

<script>
import { SuperRecord } from 'wizweb-fe'
import Mail from 'src/models/orm-api/Mail'

export default {
    name: 'Mail-read',
    components: { SuperRecord },
    computed: {
        superRecordModel() {
            return Mail
        },
    },
}
</script>

<style scoped></style>