<template>
    <div class="col-sm-6 col-sm-offset-3">
        <h1>You are Logined</h1>
    </div>
</template>

<script>
import auth from '../auth'

export default {

    data() {
        return {
            quote: ''
        }
    },

    methods: {

    },

    route: {
        canActivate() {
            return auth.user.authenticated
        }
    }

}
</script>