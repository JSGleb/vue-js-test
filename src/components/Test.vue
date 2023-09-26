<template>
    <div>
        <div v-if="num > 1">
            It's TRUE, YEAH [number = {{ num }} &gt; 1]
            <ChoiceComp />
        </div>

        <div v-else-if="num == 0">
            That's OKAY. number = {{ num }}
        </div>

        <div v-else>
            Ohh, NOO! [number = {{ num }} &lt; 1]
        </div>
    </div>
</template>

<script>
    import ChoiceComp from './Choice.vue';

    export default {
        name: 'TestComp',
        props: {
            num: Number
        },
        components: {
            ChoiceComp
        }
    }
</script>