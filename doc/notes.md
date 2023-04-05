

<script type="module">
  import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
  mermaid.initialize({ startOnLoad: true });
</script>



# Notes

- The SimReady standard as described should only be applied to static props and 3D art assets that don’t move or articulate. Why? While NVIDIA would like to provide a SimReady standard for every simulation feature immediately, that’s not practical. [source](https://docs.omniverse.nvidia.com/prod_simready/prod_simready/overview/simready-spec.html)

![semantic labelling](https://docs.omniverse.nvidia.com/prod_simready/_images/simready_taxonomy.png "Example of Semantic Labelling")


**Asset Class -> Asset Family -> Asset Category**

---
##### Materials

"By following specified SimReady material naming conventions <LINK NEEDED>, there will be tooling to help convert standard OmniPBR and OmniGlass materials into precise SimPBR physical materials that will generate the correct outputs from SimReady objects so that the RTX sensors can respond properly within the simulation." [source](https://docs.omniverse.nvidia.com/prod_simready/prod_simready/sim-needs/sensor-support.html)


##### Dimensions

"It’s important to note that all SimReady models adhere to **meter** scale for physics." [ref of Page](https://docs.omniverse.nvidia.com/prod_simready/prod_simready/sim-needs/phys-and-behaviors.html#physics-and-physical-behaviors)