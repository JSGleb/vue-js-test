<template>
    <div>
        <p v-if="response==='YES'">Да</p>
        <p v-else-if="response==='NO'">Нет</p>
        <p v-else-if="response==='MAYBE'">50/50</p>
        <p v-else>Mistake!</p>
    </div>
</template>

<script>

    export default {
        name: 'ChoiceComp',
        data() {
            return {
                response: "MAYBE"
            }
        }
    }

</script>