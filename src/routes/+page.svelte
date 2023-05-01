<script lang="ts">
  import { Node, Svelvet, Anchor } from "svelvet";
</script>

<div class="h-screen w-full">
  <Svelvet id="my-canvas" TD minimap fitView>
    <Node id="beta" bgColor="green" label="Beta">
      <div class="w-40 h-20" />
      <Anchor id="beta-anchor" />
    </Node>
    <Node
      id="alpha"
      bgColor="red"
      label="Alpha"
      let:connect
      dimensions={{ width: 400, height: 300 }}
      position={{ x: 250, y: 100 }}
    >
      <Anchor invisible />
    </Node>
  </Svelvet>
</div>
