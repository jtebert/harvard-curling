<template>
    <div class="gallery">
        <a
            v-for="(img, alt, index) in images"
            :href="img"
            :class="orientations[index]">
            <img :src="img" :alt="alt" />
        </a>
    </div>
</template>

<script>
export default {
  props: {
    images: Object,
    orientations: Array
  }
};
</script>