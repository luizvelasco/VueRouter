<template>
    <div>
        {{ $route.query.page }}
        Usuário
        <button @click="login()">
            Login
        </button>
    </div>
</template>

<script>
export default {
    created(){
        // console.log(this.$route);
        console.log(this.$router);
    },
    methods: {
        login(){
            // ajax 
            this.$router.push('/about')
            console.log('chegou');
        }
    }
}
</script>