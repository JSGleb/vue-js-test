<template>
    <!-- <div :class="{ 'active': isActive, 'disabled': isDisabled }">Классы стилей</div> -->
    <div>
        <button @click="switchBtn">Switcher</button>
        <button :class="btnClass">{{ btnText }}</button>
    </div>
</template>

<script>

    export default {
        name: 'ClasesStyles',
        data() {
            return {
                isActive: true,
                isDisabled: false,
                btnText: 'Click on me!',
            }
        },

        methods: {
            switchBtn() {
                this.isActive = !this.isActive;
                this.isDisabled = !this.isDisabled;
            }
        },

        computed: {
            btnClass() {
                return {
                    'active': this.isActive,
                    'disabled': this.isDisabled
                }
            }
        }
    }

</script>

<style>
    button {
        margin: 10px;
    }
    .active {
        background-color: darkcyan;
        color: yellow;
        padding: 10px;
    }
    
    .disabled {
        opacity: .5;
        padding: 10px;
        cursor: not-allowed;
    }
</style>