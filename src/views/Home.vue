<template>
    <div class="home">
        <img alt="Vue logo" src="../assets/logo.png">

        <!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->

        <TextVue></TextVue>
<!--        <Book></Book>-->

    </div>
</template>

<script>
    // @ is an alias to /src
    import HelloWorld from '@/components/HelloWorld.vue'
    import TextVue from '@/components/TextVue.vue'
    import Book from '@/components/Book.vue'

    export default {
        name: 'Home',
        components: {
            HelloWorld,
            TextVue,
            Book
        }
    }
</script>
