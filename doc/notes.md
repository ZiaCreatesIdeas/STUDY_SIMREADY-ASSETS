

<script type="module">
  import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
  mermaid.initialize({ startOnLoad: true });
</script>



# Notes

- The SimReady standard as described should only be applied to static props and 3D art assets that don’t move or articulate. Why? While NVIDIA would like to provide a SimReady standard for every simulation feature immediately, that’s not practical. [source](https://docs.omniverse.nvidia.com/prod_simready/prod_simready/overview/simready-spec.html)

![semantic labelling](https://docs.omniverse.nvidia.com/prod_simready/_images/simready_taxonomy.png "Example of Semantic Labelling")


```{mermaid}
flowchart LR
  A[Jupyter Notebook] --> C
  B[MyST Markdown] --> C
  C(mystjs) --> D{AST}
  D <--> E[LaTeX]
  E --> F[PDF]
  D --> G[Word]
  D --> H[React]
  D --> I[HTML]
  D <--> J[JATS]
```