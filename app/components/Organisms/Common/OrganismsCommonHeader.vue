<template>
  <div>
    <header class="header">
      <atoms-title-logo />
    </header>
  </div>
</template>

<script>
import AtomsTitleLogo from '~/components/Atoms/Title/AtomsTitleLogo';

export default {
  components: {
    AtomsTitleLogo
  }
}
</script>

<style scoped lang="scss">
  .header {
    border-bottom: 1px solid #000;

  }
</style>
