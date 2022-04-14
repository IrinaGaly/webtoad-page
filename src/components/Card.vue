<template>
  <div class="card-simple">
    <div class="card-simple__wrapper">
      <div class="card-simple__header">
        <div class="card-simple__icon-container"><component :is="icon" /></div>
        <h4 class="card-simple__title">{{ title }}</h4>
      </div>
      <p class="card-simple__description" v-html="description"></p>
    </div>
  </div>
</template>

<script>

export default {
  name: 'SectionAbout',
  props: ['icon', 'title', 'description'],
}
</script>