<script lang="ts">
  import type { Hst } from "@histoire/plugin-svelte";
  import Failed from "./Failed.svelte";
  import Ready from "./Ready.svelte";
  export let Hst: Hst;
</script>

<Hst.Story title="No Cases">
  <Hst.Variant title="Ready">
    <Ready />
  </Hst.Variant>
  <Hst.Variant title="failed">
    <Failed />
  </Hst.Variant>
</Hst.Story>
