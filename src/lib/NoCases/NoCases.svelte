<script lang="ts">
  export let title = "";
  export let subtitle = "";
  export let src = "";
</script>

<section>
  <h1>
    {title}
  </h1>
  <img {src} alt="" />
  <h2>
    {subtitle}
  </h2>
</section>

<style>
  section {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    background-color: #333;
    color: white;
    padding: 30px;
    border-radius: 16px;
    width: 350px;
    gap: 20px;
  }
  h1,
  h2 {
    all: unset;
    display: block;
  }
  h1 {
    font-weight: 700;
    font-size: 36px;
    line-height: 24px;
  }

  h2 {
    font-weight: 700;
    font-size: 16px;
    line-height: 24px;
  }
  img {
    height: 60px;
  }
</style>
