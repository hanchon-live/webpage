<template>
    <div>
        <link href='https://fonts.googleapis.com/css?family=Poppins' rel='stylesheet'>
        <b-nav>
            <b-nav-item class="font" active>Active</b-nav-item>
            <b-nav-item>Link</b-nav-item>
            <b-nav-item>Another Link</b-nav-item>
            <b-nav-item disabled>Disabled</b-nav-item>
        </b-nav>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.nav {
    margin-top:0px;
}
.nav-item {
    font-family: 'Poppins';
    font-size: 22px;
    font-weight: bold;
}
</style>