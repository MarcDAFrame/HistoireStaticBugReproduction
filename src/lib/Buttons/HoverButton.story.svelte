<script lang="ts">
  import HoverButton from "./HoverButton.svelte";
  import type { Hst } from "@histoire/plugin-svelte";
  export let Hst: Hst;

  let content = "Click Me!";
  let disabled = false;
</script>

<Hst.Story title="hover button">
  <Hst.Variant title="Normal">
    <HoverButton>Normal Button</HoverButton>
  </Hst.Variant>
  <Hst.Variant title="Disabled">
    <HoverButton disabled={true}>Disabled Button</HoverButton>
  </Hst.Variant>

  <Hst.Variant title="Controllable">
    <HoverButton {disabled}>
      {content}
    </HoverButton>
    <svelte:fragment slot="controls">
      <Hst.Text bind:value={content} title="Content" />
      <Hst.Checkbox bind:value={disabled} title="Disabled" />
    </svelte:fragment>
  </Hst.Variant>
</Hst.Story>
