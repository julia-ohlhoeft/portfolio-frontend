<template>
    <div>
        <div class="introduction">
            <h2>{{ greetings[currentGreeting] }}! 👋</h2>

            <p>Ich bin Julia quidem.</p>

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

const shuffle = (array) => {
    for (let i = array.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [array[i], array[j]] = [array[j], array[i]];
    }
    return array;
}

let greetings = [
    "Hola", "Hallo", "Hello", "Ciao", "Привет", "こんにちは",
]

greetings = shuffle(greetings)


let currentGreeting = ref(0);

function switchGreeting() {
    if (currentGreeting.value < greetings.length - 1)
        currentGreeting.value += 1;
    else currentGreeting.value = 0;
}

onMounted(() => {
    window.setInterval(() => {
        switchGreeting()
    }, 3000)
})

</script>

<style lang="scss" scoped>
.imprint-link {
    font-size: 16px;
}

h2 {
    height: 50px;
}


@media only screen and (min-width: 1000px) {
    .introduction {
        max-width: 50%;
    }
}
</style>