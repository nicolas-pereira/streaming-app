<template>
    <section>
        <button class="button is-primary"
            @click="isComponentModalActive = true">
            S'enregistrer
        </button>

        <b-modal :active.sync="isComponentModalActive" has-modal-card>
            <form action="">
            <div class="modal-card" style="width: auto">
                <header class="modal-card-head">
                    <p class="modal-card-title">S'enregistrer</p>
                </header>
                <section class="modal-card-body">
                    <b-field label="Nom de compte">
                        <b-input
                            type="text"
                            :value="username"
                            placeholder="Turbo bail"
                            required>
                        </b-input>
                    </b-field>

                    <b-field label="Email">
                        <b-input
                            type="email"
                            :value="email"
                            placeholder="Votre email"
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

                    <b-checkbox>J'accepte les turbo bails</b-checkbox>
                </section>
                <footer class="modal-card-foot">
                    <button class="button is-primary">S'enregistrer</button>
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