<template>
    <div class="hello">
        <h1>{{ msg }}</h1>

        <p v-if="seen">看到我了</p>

        <ol>
            <li v-for="todo in todos">
                {{ todo.text }}
            </li>
        </ol>


        <button @click="reverseMessage">反转消息</button>

        <p>{{ message }}</p>
        <input v-model="message">


        <p>Original message: "{{ message }}"</p>
        <p>Computed reversed message: "{{ reversedMessage }}"</p>

        <div :class="{ active: isActive}"></div>

    </div>
</template>

<script>
    export default {
        name: 'TextVue',
        data() {
            return {
                isActive: true,
                msg: 'Hello Vue.js!',
                message: 'Hello Vue!',
                seen: true,
                todos: [
                    { text: '学习 JavaScript' },
                    { text: '学习 Vue' },
                    { text: '整个牛项目' }
                ]
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

<style>














</style>

