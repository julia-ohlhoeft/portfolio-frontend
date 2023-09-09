<template>
    <div>
        <div class="introduction">
            <h2>Hola! 👋</h2>

            <p>Ich bin Julia Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo sed nobis dolore. Sapiente
                perspiciatis dignissimos culpa laudantium. Sequi voluptas dignissimos tempore illum asperiores doloribus
                iusto, tempora tenetur molestias ullam quidem.</p>

            <br>
            <p> You can find me on <nuxt-link to="https://www.pinterest.de/ju_35mm_film/">Pinterest</nuxt-link></p>
        </div>
        <nuxt-link class="imprint-link" to="/imprint">Imprint</nuxt-link>
    </div>
</template>

<script setup>
useHead({
    title: 'Julia Ohlhöft',
    meta: [
        { name: 'description', content: 'Portfolio of Julia Ohlhöft' }
    ],

})
</script>

<style lang="scss" scoped>
.imprint-link {
    font-size: 16px;
}



@media only screen and (min-width: 1000px) {
    .introduction {
        max-width: 50%;
    }
}
</style>