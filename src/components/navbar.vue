<template>
    <b-navbar>
        <template #brand>
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                Turbo Streaming
            </b-navbar-item>
        </template>
        <template #start>
            <b-navbar-item href="#">
                Acceuil
            </b-navbar-item>
            <b-navbar-dropdown label="Info">
                <b-navbar-item href="#">
                    À propos
                </b-navbar-item>
                <b-navbar-item href="#">
                    Contact
                </b-navbar-item>
            </b-navbar-dropdown>
        </template>

        <template #end>
            <b-navbar-item tag="div">
                <div class="buttons">
                    <register></register>
                    <login></login>
                </div>
            </b-navbar-item>
        </template>
    </b-navbar>
</template>

<script>
import login from './login.vue'
import register from './register.vue'

export default {
    components: {
        login,
        register
    }
}
</script>

<style>

</style>