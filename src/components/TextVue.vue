<template>
    <div class="hello">
        <h1>{{ msg }}</h1>
        
        <p v-if="seen">看到我了</p>
        
    </div>
</template>

<script>
    export default {
        name: 'TextVue',
        data() {
            return {
                msg: 'fffff',
                seen: true
            }
        }
    }
</script>

