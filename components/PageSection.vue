<template>
<section :id="id">
    <header>
        <h3 v-if="isSubsection">{{ title }}</h3>
        <h2 v-else>{{ title }}</h2>
        <p v-if="description">{{ description }}</p>
    </header>
    <div class="content">
        <slot></slot>
    </div>
    <footer v-if="hasFooterSlot">
        <slot name="footer"></slot>
    </footer>
</section>
</template>

<script>
export default {
  props: {
    title: String,
    id: String,
    description: String,
    isSubsection: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    hasFooterSlot() {
      return !!this.$slots["footer"] || !!this.$scopedSlots["footer"];
    }
  }
};
</script>