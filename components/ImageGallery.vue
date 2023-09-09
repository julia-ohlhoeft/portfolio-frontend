<template>
    <div>

    </div>
</template>

<script setup>

defineProps({
    imagePath: { type: String }
})


let currentImage = ref(0);

const images = [

    '@/assets/images/image-1.jpg',
    '@/assets/images/image-2.jpg',
    "@/assets/images/image-3.jpg",
    "@/assets/images/image-4.jpg",
]


/* function switchImage() {
    if (currentImage.value < images.length)
        currentImage.value += 1;
    else currentImage.value = 0;
}

onMounted(() => {
    window.setInterval(() => {
        switchImage()
    }, 10000)
}) */


</script>

<style lang="scss" scoped>
img {
    max-height: 400px;
    object-fit: contain;
    object-position: center;
}
</style>