<template>
    <div class="layout">

        <div class="page-content">
            <slot></slot>
        </div>
        <!-- <Footer></Footer> -->
    </div>
</template>

<script setup>

</script>

<style lang="scss">
@font-face {
    font-family: montserrat;
    src: url(~/assets/fonts/Montserrat-VariableFont_wght.ttf);
}

body {
    margin: 0;
}

.page-content {
    flex: 1;
}

.layout {
    display: flex;
    flex-direction: column;
    width: calc(100% - 100px);
    margin: auto;
    margin-top: 40px;
    margin-bottom: 0;
    /*   min-height: 100vh; */

    font-family: montserrat;
    font-size: large;
}

a {
    //text-decoration: none;
    /* color: black;  */
    color: blue;

    &:visited {
        color: blue;
    }

    &:hover {
        font-weight: 500;
    }
}

ul {
    margin: 0;
    padding: 0;
}

li {
    list-style-type: none;
}
</style>