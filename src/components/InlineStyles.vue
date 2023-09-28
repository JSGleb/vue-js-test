<template>
    <div :style="customStyles">Inline-стили</div>
</template>

<script>

export default {
    name: 'InlineStyles',

    computed: {
        customStyles() {
            return {
                backgroundColor: 'lightblue',
                color: 'brown',
                fontSize: '32px',
                fontStyle: 'bold',
                padding: '20px',
                marginTop: '15px'
            }
        }
    }
}

</script>