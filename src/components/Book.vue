<template>
    <div class="hello">
        <p>
            Ask a yes/no question:
            <input v-model="question">
        </p>
        <p>{{ answer }}</p>

    </div>
</template>

<script>
    export default {
        name: 'Book',
        data() {
            return {
                question: '',
                answer: 'I cannot give you an answer until you ask a question!'
            }
        },
        computed: {
            ///
            reversedMessage: function () {
                return this.message.split('').reverse().join('')
            }

        },
        methods: {
            reverseMessage: function () {
                this.msg = this.msg.split('').reverse().join('')
            }
        }




    }
</script>

