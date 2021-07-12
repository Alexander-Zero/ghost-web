<template>
    <div class="login-form  opacity-8 radius8">
        <br/><br/>
        <h2>账号登录</h2><br/>
        <el-input class="login-input" v-model="username" placeholder="账号"></el-input>
        <br/>
        <br/>
        <el-input class="login-input" v-model="password" placeholder="密码" show-password></el-input>
        <br/>
        <br/>
        <el-button class="login-input">登录</el-button>

    </div>

</template>

<script>
    import InputIcon from "../../components/common/InputIcon";

    export default {
        data() {
            return {
                password: "",
                username: ""
            }
        },
        name: "LoginForm",
        components: {InputIcon}
    }
</script>

<style scoped>
    .login-form {
        width: 400px;
        height: 450px;
        background: white;
        position: relative;
        left: 400px;
    }

    .login-input {
        width: 300px;
    }


</style>