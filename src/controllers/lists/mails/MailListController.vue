<template>

    <div>
        <mailList
            :parentKeyValuePair="parentKeyValuePair"
            :fetchFlags="fetchFlags"
        />
    </div>
</template>

<script>
import mailList from 'src/views/lists/mails/MailList.vue'

export default {
    name: 'Mail-list-controller',
    components: {
        mailList,
    },

    data() {
        return {
            parentKeyValuePair: {},
            fetchFlags: {}
        }
    },
}
</script>