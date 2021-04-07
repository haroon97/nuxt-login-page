<template>
    <div class="background">
        <section class="section">
            <div class="block">
                <h3 class="title is-2">Welcome Back</h3>
                <p class="subtitle is-6">Thank you for getting back, please login to your account by filling these form</p>
            </div>
            <b-field label="Email Address">
                <b-input placeholder="Email"
                    type="email"
                    custom-class="borderless"
                    icon="account">
                </b-input>
            </b-field>
            <b-field label="Password">
                <b-input placeholder="Password"
                    password-reveal
                    type="password"
                    custom-class="borderless"
                    icon="lock">
                </b-input>
            </b-field>
            <b-field>
                <b-checkbox size="is-small">Remember me</b-checkbox>
            </b-field>
            <b-button class="btn">LOGIN</b-button>
        </section>
    </div>
</template>

<script>

export default {
    data() {
        return {
            email: '',
            password: '',
        }
    }
}
</script>

<style>
    .background {
        display: flex;
        align-items: center;
        height: 100vh;
        background-image: url('~/assets/background.png');
        background-repeat: no-repeat;
        background-position: right;
        background-size: contain;
    }
    .section {
        width: 50%;
        padding-left: 5rem;
    }
    .borderless {
        border-top-style: none;
        border-right-style: none;
        border-left-style: none;
        box-shadow: none;
    }
    .borderless:active {
        border-top-style: none;
        border-right-style: none;
        border-left-style: none;
        box-shadow: none;
    }
    .btn {
        padding-left: 4rem;
        padding-right: 4rem;
        border-radius: 100px;
        background-color: #34d8eb;
        color: white;
    }
    .title {
        color: #34d8eb;
    }
    .subtitle {
        max-width: 65%;
        color: grey;
    }
</style>
