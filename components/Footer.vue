<template>
    <footer>
        <ul>
            <li><nuxt-link to="/">Home</nuxt-link></li>
            <li><nuxt-link to="/imprint">Imprint</nuxt-link></li>
            <!-- <li><nuxt-link to="privacy policy">Privacy Policy</nuxt-link></li> -->
        </ul>
    </footer>
</template>

<script setup>

</script>

<style lang="scss" scoped>
footer {
    margin-top: 30px;
    height: 50px;

    font-size: 16px;



    /* border-top: 1px solid black; */

    ul {
        display: flex;

        li {

            margin-right: 30px;
        }
    }
}
</style>