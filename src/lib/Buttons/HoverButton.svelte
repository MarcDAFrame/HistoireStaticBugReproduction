<script lang="ts">
</script>

<button {...$$restProps}>
  <slot />
</button>

<style lang="scss">
  button {
    all: unset;
    display: block;
    cursor: pointer;
    box-sizing: border-box;
    width: 100%;
    height: 43px;
    background-color: #f1a04d;
    border: 1px solid #f1a04d;
    border-radius: 8px;
    padding: 8px 8px;
    font-size: 18px;
    line-height: 150%;
    color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
    transition: all 0.3s ease;

    &:hover {
      background-color: #4f4f4f;
    }

    &:disabled {
      background-color: #4f4f4f;
      border: 1px solid #bdbdbd;
      cursor: not-allowed;
    }
  }
</style>
