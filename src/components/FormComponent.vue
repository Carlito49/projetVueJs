<template>
<form method="POST" @submit.prevent="checkLogin">
    <div class="row">
        <div class="d-flex justify-content-around mb-3">
            <div class="col-3">
                <label for="username">Entrez votre nom d'utilisateur :</label>
            </div>
            <div class="col-4">
                <input type="text" id="username" name="username" class="w-100" v-model="login"/>
            </div>
        </div>
        <div class="d-flex justify-content-around mb-3">
            <div class="col-3">
                <label for="password">Entrez votre mot de passe :</label>
            </div>
            <div class="col-4">
                <input type="password" id="password" name="password" class="w-100" v-model="password"/>
            </div>
        </div>
        <div class="d-flex justify-content-center">
            <button type="submit" class="btn btn-primary w-25">Valider</button>
        </div>
    </div>
</form>
</template>

<script lang="ts">
    import router from '@/router';
    import { Component, Vue, Prop } from 'vue-property-decorator';

    export default {
        data: () => ({
            
        }),
        props: {
            login: String,
            password: String
        },
        methods: {
            checkLogin(): void {
                if(this.login === "admin" && this.password === "admin") {
                    router.push({ path: '/about' })
                }
            }
        }
    }
    
</script>

<style>

</style>
