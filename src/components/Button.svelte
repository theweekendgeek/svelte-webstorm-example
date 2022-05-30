<script lang="ts">
  export let title = '';
  export let handleClick: CallableFunction;

  const onClick = () => {
    if (!handleClick) {
      console.warn(`no handleClick Method passed to button with title ${title}`);
      return;
    }

    handleClick();
  };
</script>

<button on:click|preventDefault={onClick}> {title} </button>

<style lang="scss">
  @import '../styles/colors.scss';

  button {
    background: $secondary;
  }
</style>
