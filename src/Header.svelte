<script>
  export let color = "primary"  ;
</script>

<style>
  div {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    font-size: 50px;
    letter-spacing: 5px;
    transition: color 2000ms ease 0ms;
  }

  .primary {
    color: var(--primary-color);
  }

  .secondary {
    color: var(--secondary-color);
  }

  .tertiary {
    color: var(--tertiary-color);
  }

  .quarnary {
    color: var(--quarnary-color);
  }
</style>

<div class="{color}"><slot /></div>
