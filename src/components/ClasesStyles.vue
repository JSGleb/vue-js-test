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
            btnText: 'Click on me!'
        }
    },

    methods: {
        switchBtn() {
            this.isActive = !this.isActive;
            this.isDisabled = !this.isDisabled;
            console.log(this.isActive)
            console.log(this.isDisabled)
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

<style scoped>

    button:nth-of-type(2) {
        font-size: 2em;
        width: 100%;
        padding: 20px;
    }
    .active {
        background-color: darkcyan;
        color: yellowgreen;
        cursor: pointer;
        transition: all .4s ease-in;
    }
    .active:hover {
        background-color: red;
    }

    .disabled {
        opacity: .5;
        padding: 20px;
        cursor: not-allowed;
    }
</style>