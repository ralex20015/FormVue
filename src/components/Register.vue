<script>
export default{
    data(){
        return{
            users: []
        }
    },
    methods: {
        addUser(){
            this.users.push(
                {
                    name: this.name,
                    username: this.username,
                    email: this.email,
                    password: this.password
                }
            );
            localStorage.setItem("users", JSON.stringify(this.users));
        }
    }
}
</script>

<template>
    <h2>Register now</h2>
    <form action="" id="form">
        <div>
            <label for="name">Name</label>
            <input type="text" name="name" id="name" v-model="name">
            <label for="username">Username</label>
            <input type="text" name="username" id="username" v-model="username">
            <label for="email">Email</label>
            <input type="email" name="email" id="email" v-model="email">
            <label for="pass">Password</label>
            <input type="password" name="pass" id="pass" v-model="password">
            <button type="submit" class="btn" @click="addUser">Register</button>
        </div>
    </form>
</template>

<style>

</style>