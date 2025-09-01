<template>
    <div class="login-container">
        <form class="login-form" @submit.prevent="login">
            <h2>Login</h2>
            <div class="form-group">
                <label for="username">Username</label>
                <input v-model="username" type="text" id="username" required />
            </div>
            <div class="form-group">
                <label for="password">Password</label>
                <input v-model="password" type="password" id="password" required />
            </div>
            <button type="submit">Login</button>
        </form>
    </div>
</template>

<script>
export default {
    name: "Login",
    data() {
        return {
            username: "",
            password: ""
        };
    },
    methods: {
        login() {
            // Placeholder for login logic
            alert(`Username: ${this.username}\nPassword: ${this.password}`);
        }
    }
};
</script>

<style scoped>
.login-container {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: #f5f6fa;
}

.login-form {
    background: #fff;
    padding: 2rem 2.5rem;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    width: 320px;
}

.login-form h2 {
    margin-bottom: 1.5rem;
    text-align: center;
    color: #333;
}

.form-group {
    margin-bottom: 1rem;
}

.form-group label {
    display: block;
    margin-bottom: 0.5rem;
    color: #555;
}

.form-group input {
    width: 100%;
    padding: 0.5rem;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 1rem;
}

button[type="submit"] {
    width: 100%;
    padding: 0.75rem;
    background: #1976d2;
    color: #fff;
    border: none;
    border-radius: 4px;
    font-size: 1rem;
    cursor: pointer;
    transition: background 0.2s;
}

button[type="submit"]:hover {
    background: #1565c0;
}
</style>