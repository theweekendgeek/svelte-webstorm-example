<script lang="ts">
  export let title: string = '';
</script>

<button> {title} </button>

<style lang="scss">
  @import '../styles/colors.scss';

  button {
    background: $secondary;
  }
</style>
