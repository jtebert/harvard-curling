<template>
<section class="intro">
    <header>
        <h1>{{ title }}</h1>
        <span class="image main" id="logo"><img :src="logo" alt="Site logo" /></span>
        <p v-html="intro"></p>
        <ul class="actions">
            <li><a :href="scrollTo" class="arrow scrolly"><span class="label">Next</span></a></li>
        </ul>
    </header>
    <div class="content">
        <span class="image fill" data-position="center"><img :src="img" alt="" /></span>
    </div>
</section>
</template>

<script>
export default {
  props: {
    title: String,
    logo: String,
    intro: String,
    img: String,
    scrollTo: {
      type: String,
      default: "#about"
    }
  }
};
</script>