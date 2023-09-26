<template>
    <div :style="customStyles">Inline-Стили</div>
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
                    padding: '10px',
                    marginTop: '15px'
                }
            }
        }
    }

</script>