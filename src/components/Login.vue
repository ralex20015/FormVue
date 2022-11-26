<script>

</script>

<template>
    <h2>Login in your acount</h2>
    <form action="">
        <div>
            <label for="username">Username</label>
            <input type="text" name="username" id="username">
            <label for="password">Password</label>
            <input type="text" name="password" id="password">
            <button type="submit" class="btn">Login</button>
            <p>I've an <a href="#">acount</a></p>
        </div>
    </form>
</template>

<style>
h2 {
    text-align: center;
}

form {
    padding: 10px;
    width: 40%;
    margin-left: 30%;
    margin-right: 30%;
    display: flex;
    flex-direction: column;
}

form div{
    width: 50%;
    margin-left: 25%;
    margin-right: 25%;
    display: flex;
    flex-direction: column;
}

form div input{
    height: 1.5rem;
}

form div p{
    text-align: center;
}

.btn {
    height: 2rem;
    padding: 5px;
    margin: 10px 0;
    background-color: #0f4f0f;
    border: 1px solid rgba(255, 255, 255, 0.5);
    border-radius: 10px;
}
</style>