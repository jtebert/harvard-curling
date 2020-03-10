<template>
<li>
    <h3><slot></slot></h3>
    <a v-if="links" v-for="(name, value, index) in links" :href="value">
      <br v-if="index != 0">{{ name }}
    </a>
    <ul v-if="socialLinks" class="icons">
      <li v-for="(link, icon) in socialLinks">
        <a
            :href="link"
            :class="['icon', 'brands', 'fa-'+icon]">
            <span class="label">{{ icon }}</span>
        </a>
      </li>
    </ul>
</li>
</template>

<script>
export default {
  props: {
    links: Object,
    socialLinks: Object
  }
};
</script>