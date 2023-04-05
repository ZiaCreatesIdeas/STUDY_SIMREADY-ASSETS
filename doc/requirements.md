


# Requirements

## Workflow
**Physical Creation**
- Gather references.
- Model
    * Chamfers / Bevels
    * Ngons <= 4, triangles are ok
      
- Texture
    * UV's may need to follow grain
    * Materials should include wear. 
- Naming 
    *  Each object follows naming convention
- Rigging
    * Create Dummy Object to parent Prims to. 
      
**Sim Preparation**
- Check Assembly
    * Avoid nested Gprims, no direct parenting of assets.
    * Material Naming (3 part core naming convention)
    * Ensure 'Z' up orientation.
- Conform file names and types to be Synthetic Generator Friendly
    * Use USD composition arcs. 
    * Save Geometry to an 'Instance' / Inst file. (27:10) [source](https://www.nvidia.com/gtc/session-catalog/?search=beau&tab.catalogallsessionstab=16566177511100015Kus&search=beau#/session/1674663459922001qgvS)
    * Add Inst file as Reference in new file, not payload.       
    New File > Preferences Tab > Stage Label > Import > **'Payload' => 'References'**
    
    

- SimReady 3D art assets must include rigid-body physics pre-configured by default so that they can be inserted into a scene quickly and immediately interact with other elements. [source](https://docs.omniverse.nvidia.com/prod_simready/prod_simready/sim-needs/phys-and-behaviors.html#physics-and-physical-behaviors)  

### Common Modeling issues and Recommended Solution

[source](https://docs.omniverse.nvidia.com/prod_simready/prod_simready/simready-asset-creation/modeling-issues.html)

- NGons.  

::::{important}
:::{note}
This text is **standard** _Markdown_
:::
:::: 

<div class="admonition note" name="html-admonition" style="background: lightgreen; padding: 10px">
<p class="title">This is the **title**</p>
This is the *content*
</div>