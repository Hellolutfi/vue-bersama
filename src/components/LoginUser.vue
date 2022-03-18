<template>
    <div>
        <form>
            <input type="text" v-model="username" placeholder="Username">
            <input type="password" v-model="password" placeholder="Password">
            <button type="button" @click="login">Login</button>
        </form>
    </div>
</template>

<script>
export default {
    name: 'LoginUser',
    data() {
        return {
            username: '',
            password: ''
        }
    },
    methods: {
        login() {
            console.log(this.username, this.password);
        }
    }
}
</script>