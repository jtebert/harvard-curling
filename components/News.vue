<template>
<div>
    <h2><a :href="link">{{ title }}</a></h2>
    <p>{{ source }}</p>
    <span v-if="img" class="image main"><img :src="img" :alt="alt"></span>
    <div v-else-if="video" class="videoWrapper">
        <iframe width="560" height="315" :src="video" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
</div>
</template>

<script>
export default {
  props: ["title", "link", "source", "img", "alt", "video"]
};
</script>