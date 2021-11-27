<template>
    <section>
        <button class="button is-light"
            @click="isComponentModalActive = true">
            Se connecter
        </button>

        <b-modal :active.sync="isComponentModalActive" has-modal-card>
            <form action="">
            <div class="modal-card" style="width: auto">
                <header class="modal-card-head">
                    <p class="modal-card-title">Se connecter</p>
                </header>
                <section class="modal-card-body">
                    <b-field label="Nom d'utilisateur">
                        <b-input
                            type="text"
                            :value="username"
                            placeholder="Turbo bail"
                            required>
                        </b-input>
                    </b-field>

                    <b-field label="Mot de passe">
                        <b-input
                            type="password"
                            :value="password"
                            password-reveal
                            placeholder="Vote mot de passe"
                            required>
                        </b-input>
                    </b-field>

                    <b-checkbox>Se souvenir de moi</b-checkbox>
                </section>
                <footer class="modal-card-foot">
                    <button class="button is-primary">Se connecter</button>
                </footer>
            </div>
        </form>
        </b-modal>
    </section>
</template>

<script>
export default {
    data() {
        return {
            isComponentModalActive: false,
        }
    }
}
</script>

<style>

</style>