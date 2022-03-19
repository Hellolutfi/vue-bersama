<template>
    <div class="register">
        <h1>Register</h1>
        <form @submit.prevent="register">
            <div class="form-group">
                <label for="name">Name</label>
                <input type="text" class="form-control" id="name" v-model="name">
            </div>
            <div class="form-group">
                <label for="email">Email</label>
                <input type="email" class="form-control" id="email" v-model="email">
            </div>
            <div class="form-group">
                <label for="password">Password</label>
                <input type="password" class="form-control" id="password" v-model="password">
            </div>
            <button type="submit" class="btn btn-primary">Register</button>
        </form>
    </div>
</template>
<script>
export default {
    name: 'RegisterUser',
    data() {
        return {
            name: '',
            email: '',
            password: ''
        }
    },
    methods: {
        register() {
            console.log('Registering user...');
            console.log(this.name);
            console.log(this.email);
            console.log(this.password);
        }
    }
}
</script>