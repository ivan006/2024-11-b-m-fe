<template>

    <div>
        <q-card class="q-mb-md">
            <mailRead :id="id" />
        </q-card>
    </div>
</template>

<script>
import mailRead from 'src/views/lists/mails/MailRead.vue'

export default {
    name: 'Mail-read-controller',
    components: {
        mailRead,
    },

    data() {
        return {
            id: +this.$route.params.rId
        }
    },
}
</script>