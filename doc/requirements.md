


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


| Time | Information |
|------|-------------|
| 0:00 | Learn to use Simready assets by focusing on the with physics.usd file which has all necessary physics attributes. |
| 0:22 | To work with the assets in the physics scene, set one meter as one unit and use 9.8 gravity. Add the with physics dot USD file by dragging it in. |
| 0:46 | Dragging the file in brings in a payload, instancing a reference and a physics material. Press play to get physics and shift+drag to move objects around. |
| 1:19 | Simready assets come with all necessary elements pre-canned. Each asset has a main transform with meshes that can be for render or collision messages. |
| 2:00 | The main transform has rigid body properties that can be enabled or disabled, and linear and angular velocity can be added. Keep masses and densities to Auto compute to consider the physics material. |
| 2:41 | Each mesh has collider properties that can be enabled or disabled. To view the object colliding with the collider, go to the eyeball and select physics, then colliders, and show all. |
| 3:18 | Sim-ready assets usually have efficient colliders set up, but if needed, go to approximation to adjust options for efficiency. |

---

| Time Code | Sentences |
| --- | --- |
| 0:00 | Hey everybody here's a quick tutorial on how to use simrani assets. |
| 0:05 | When you go into a Sim ready folder, you're going to see numerous files. |
| 0:08 | We're going to focus on the with physics.usd file. |
| 0:10 | The with physics.usd file is everything needed to simulate this asset with rigid bodies. |
| 0:19 | The file is only the physics attributes referencing the inst file. |
| 0:22 | I started this scene just by doing new from stage template and bringing the abandoned parking lot, and then I also added a physics scene. |
| 0:30 | This is very important because based on what unit you're working in and right now we're going to work in one meter is one unit, and that's how all simulator assets are going to be processed. |
| 0:43 | So our gravity is going to actually be 9.8. |
| 0:46 | Now I'm going to drag in my with physics dot USD. |
| 0:57 | When you look at this, we have a payload and we're instancing a referencing, sorry, the inst file, and we have a physics material. |
| 1:06 | Put this anywhere and press the play button. |
| 1:09 | Now we get physics, we can also hit shift and drag these around. |
| 1:19 | Maybe I want to duplicate this one. |
| 1:29 | And press play and now we got these guys stacking pretty nicely. |
| 1:38 | The simrani assets are going to come already pre-canned with any of this stuff. |
| 1:40 | Let's get into a little bit about how the asset is organized. |
| 1:48 | Like I said before, we have a payload and then we have a reference to the model, and then inside there we're going to have one main transform always, and underneath there we'll have our meshes. |
| 2:03 | So all of our rigid body properties are going to be on this main transform. |
| 2:10 | When we look in the property editor we should see rigid body and then here you can disable or enable it, you can also check this if you want to keyframe it, okay, and if you want to add some linear velocity this is initial lineography and initial angular velocity can do from here. |
| 2:33 | Usually you're not going to mess with a whole lot in this area. |
| 2:36 | We want to keep our masses and densities and everything to Auto compute because it's going to take in account the physics material. |
| 2:45 | Each mesh is actually going to have the Collision the collider properties. |
| 2:52 | If you want to see how this object with the Collision object is for this, you're going to go to this eyeball here, you're going to show type down in physics, you can see colliders and we're going to show all. |
| 3:04 | Now you can see we got this pink wireframe. |
| 3:09 | We want to make these as efficient as possible so we get some options down in the Collider. |
| 3:16 | Usually a Sim ready asset is going to already have this stuff set up, but if you wanted to come in here and make something even

---

| Time Code | Sentences                                                                                                    | YouTube Link with Start Time                            | Link as Markdown Code                                                   |
|----------|--------------------------------------------------------------------------------------------------------------|--------------------------------------------------------|--------------------------------------------------------------------------|
| 2:52     | If you want to see how this object with the Collision object is for this, you're going to go to this eyeball here, you're going to show type down in physics, you can see colliders and we're going to show all.  | https://youtu.be/lFtEMg86lJc?t=172 | [Link](https://youtu.be/lFtEMg86lJc?t=172) |
| 3:04     | Now you can see we got this pink wireframe.                                                                   | https://youtu.be/lFtEMg86lJc?t=184                     | `[Link](https://youtu.be/lFtEMg86lJc?t=184)`                            |
| 3:09     | We want to make these as efficient as possible so we get some options down in the Collider.                  | https://youtu.be/lFtEMg86lJc?t=189                     | `[Link](https://youtu.be/lFtEMg86lJc?t=189)`                             |
| 3:16     | Usually a Sim ready asset is going to already have this stuff set up, but if you wanted to come in here and make something even    | https://youtu.be/lFtEMg86lJc?t=196   | `[Link](https://youtu.be/lFtEMg86lJc?t=196)`                         |

---

| Time Code | Sentences                                                                                                     | YouTube Link with Start Time                          |
|-----------|----------------------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| 2:52      | If you want to see how this object with the Collision object is for this, you're going to go to this eyeball... | [https://youtu.be/lFtEMg86lJc?t=172](172)            |
| 3:04      | Now you can see we got this pink wireframe.                                                                     | [https://youtu.be/lFtEMg86lJc?t=184](184)            |
| 3:09      | We want to make these as efficient as possible so we get some options down in the Collider.                     | [https://youtu.be/lFtEMg86lJc?t=189](189)            |
| 3:16      | Usually a Sim ready asset is going to already have this stuff set up, but if you wanted to come in here an... | [https://youtu.be/lFtEMg86lJc?t=196](196)            |

---

| Time Code | Sentences | YouTube Link with Start Time |
|-----------|-----------|------------------------------|
| 2:52 | If you want to see how this object with the Collision object is for this, you're going to go to this eyeball here, you're going to show type down in physics, you can see colliders and we're going to show all. | [Link](https://youtu.be/lFtEMg86lJc?t=172) |
| 3:04 | Now you can see we got this pink wireframe. | [Link](https://youtu.be/lFtEMg86lJc?t=184) |
| 3:09 | We want to make these as efficient as possible so we get some options down in the Collider. | [Link](https://youtu.be/lFtEMg86lJc?t=189) |
| 3:16 | Usually a Sim ready asset is going to already have this stuff set up, but if you wanted to come in here and make something even | [Link](https://youtu.be/lFtEMg86lJc?t=196) |

---

| Time Code | Sentences | Video |
| --- | --- | --- |
| 2:52 | If you want to see how this object with the Collision object is for this, you're going to go to this eyeball here, you're going to show type down in physics, you can see colliders and we're going to show all. | [2:52](https://youtu.be/lFtEMg86lJc?t=172) |
| 3:04 | Now you can see we got this pink wireframe. | [3:04](https://youtu.be/lFtEMg86lJc?t=184) |
| 3:09 | We want to make these as efficient as possible so we get some options down in the Collider. | [3:09](https://youtu.be/lFtEMg86lJc?t=189) |
| 3:16 | Usually a Sim ready asset is going to already have this stuff set up, but if you wanted to come in here and make something even | [3:16](https://youtu.be/lFtEMg86lJc?t=196) |

---

| Time Code | Information | Video Reference |
|-----------|-------------|-----------------|
| 5:08 | Importance of scaling objects and adjusting the density attribute when working with rigid bodies in a physics engine is noted. | https://youtu.be/lFtEMg86lJc?t=308 |
| 5:13 | Density attribute is mentioned as determining masses, which are essential when working with rigid bodies. | https://youtu.be/lFtEMg86lJc?t=313 |
| 5:21 | Suggestion to have a physics asset in each folder to define an object's physical properties. | https://youtu.be/lFtEMg86lJc?t=321 |
| 5:29 | The speaker drags the physics asset into the folder. | https://youtu.be/lFtEMg86lJc?t=329 |
| 5:39 | Other tutorials are suggested to learn about additional features that come with physics assets, such as semantic labeling. | https://youtu.be/lFtEMg86lJc?t=339 |
| 5:46 | The speaker thanks the audience for watching. | https://youtu.be/lFtEMg86lJc?t=346 |

---

| Time Code | Information | Video Reference |
|-----------|-------------|-----------------|
| 5:08 | Importance of scaling objects and adjusting the density attribute when working with rigid bodies in a physics engine is noted. | ![5:08](https://youtu.be/lFtEMg86lJc?t=308) |
| 5:13 | Density attribute is mentioned as determining masses, which are essential when working with rigid bodies. | ![5:13](https://youtu.be/lFtEMg86lJc?t=313) |
| 5:21 | Suggestion to have a physics asset in each folder to define an object's physical properties. | ![5:21](https://youtu.be/lFtEMg86lJc?t=321) |
| 5:29 | The speaker drags the physics asset into the folder. | ![5:29](https://youtu.be/lFtEMg86lJc?t=329) |
| 5:39 | Other tutorials are suggested to learn about additional features that come with physics assets, such as semantic labeling. | ![5:39](https://youtu.be/lFtEMg86lJc?t=339) |
| 5:46 | The speaker thanks the audience for watching. | ![5:46](https://youtu.be/lFtEMg86lJc?t=346) |

---

| Time Code | Information | Video Reference |
|-----------|-------------|-----------------|
| 5:08 | Importance of scaling objects and adjusting the density attribute when working with rigid bodies in a physics engine is noted. | [5:08](https://youtu.be/lFtEMg86lJc?t=308) |
| 5:13 | Density attribute is mentioned as determining masses, which are essential when working with rigid bodies. | [5:13](https://youtu.be/lFtEMg86lJc?t=313) |
| 5:21 | Suggestion to have a physics asset in each folder to define an object's physical properties. | [5:21](https://youtu.be/lFtEMg86lJc?t=321) |
| 5:29 | The speaker drags the physics asset into the folder. | [5:29](https://youtu.be/lFtEMg86lJc?t=329) |
| 5:39 | Other tutorials are suggested to learn about additional features that come with physics assets, such as semantic labeling. | [5:39](https://youtu.be/lFtEMg86lJc?t=339) |
| 5:46 | The speaker thanks the audience for watching. | [5:46](https://youtu.be/lFtEMg86lJc?t=346) |

---

| Time Code | Information | Video Link |
|-----------|-------------|------------|
| 5:08 | If you scale these objects and work in different units, you're going to have to scale this density attribute because  
|      | it's determining your masses and we're looking at the rigid bodies. Obviously, your masses are super important, right? | [![5:08](https://img.youtube.com/vi/lFtEMg86lJc/0.jpg)](https://www.youtube.com/watch?v=lFtEMg86lJc&t=5m8s) |
| 5:21 | So again, any of these folders, we should have a physics asset. | [![5:21](https://img.youtube.com/vi/lFtEMg86lJc/1.jpg)](https://www.youtube.com/watch?v=lFtEMg86lJc&t=5m21s) |
| 5:29 | And here, drag this in. | [![5:29](https://img.youtube.com/vi/lFtEMg86lJc/2.jpg)](https://www.youtube.com/watch?v=lFtEMg86lJc&t=5m29s) |
| 5:39 | They should already pre-cam and look at some other tutorials for some of the other things that come with similarity acids, like semantic labeling. | [![5:39](https://img.youtube.com/vi/lFtEMg86lJc/3.jpg)](https://www.youtube.com/watch?v=lFtEMg86lJc&t=5m39s) |
| 5:46 | Thank you for watching. | [![5:46](https://img.youtube.com/vi/lFtEMg86lJc/4.jpg)](https://www.youtube.com/watch?v=lFtEMg86lJc&t=5m46s) |

---

 [![5:29](https://img.youtube.com/vi/lFtEMg86lJc/2.jpg)](https://www.youtube.com/watch?v=lFtEMg86lJc&t=0m34s) |
 
---

| Time Code | Information | 
| --- | --- |
| [0:00](https://youtu.be/lFtEMg86lJc?t=0s) | Open a Sim ready folder and locate the with physics.usd file. |
| [0:22](https://youtu.be/lFtEMg86lJc?t=22s) | Create a new scene using the abandoned parking lot template and add a physics scene. |
| [0:30](https://youtu.be/lFtEMg86lJc?t=30s) | Set the unit system to one meter per unit. |
| [0:46](https://youtu.be/lFtEMg86lJc?t=46s) | Drag the with physics.usd file into the scene. |
| [0:54](https://youtu.be/lFtEMg86lJc?t=54s) | Check that the payload and inst file are referencing properly and that a physics material is present. |
| [1:06](https://youtu.be/lFtEMg86lJc?t=1m6s) | Press the play button to enable physics simulation. |
| [1:09](https://youtu.be/lFtEMg86lJc?t=1m9s) | Use the shift key to drag and move objects around in the simulation. |

---

| Time code | Description |
|-----------|-------------|
| ![0:00](https://img.youtube.com/vi/lFtEMg86lJc/0.jpg) | Introduction |
| ![1:14](https://img.youtube.com/vi/lFtEMg86lJc/1.jpg) | Stop the simulation and go back to the beginning. |
| ![1:16](https://img.youtube.com/vi/lFtEMg86lJc/2.jpg) | Duplicate one of the objects. |
| ![1:17](https://img.youtube.com/vi/lFtEMg86lJc/3.jpg) | Optionally rotate the duplicated object. |
| ![1:19](https://img.youtube.com/vi/lFtEMg86lJc/4.jpg) | Press play and observe the stacked objects. |
| ![1:29](https://img.youtube.com/vi/lFtEMg86lJc/5.jpg) | Manipulate the stacked objects as desired. |
| ![1:38](https://img.youtube.com/vi/lFtEMg86lJc/6.jpg) | Simready assets come pre-packaged with these features. |
| ![1:43](https://img.youtube.com/vi/lFtEMg86lJc/7.jpg) | Simready assets are organized with a payload and a reference to the model. |
| ![1:54](https://img.youtube.com/vi/lFtEMg86lJc/8.jpg) | Inside, there is always one main transform, underneath which are the meshes. |
| ![2:00](https://img.youtube.com/vi/lFtEMg86lJc/9.jpg) | These meshes can be for rendering or collision detection. |
| ![2:06](https://img.youtube.com/vi/lFtEMg86lJc/10.jpg) | Rigid body properties are located on the main transform. |

---

<div style="width: 80%; overflow-x: auto;">
| Time Code | Description |
|-----------|-------------|
| <iframe width="400" height="226" src="https://www.youtube.com/embed/lFtEMg86lJc?start=74&modestbranding=1&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> 1:14 | Stop the simulation and go back to the beginning. |
| <iframe width="400" height="226" src="https://www.youtube.com/embed/lFtEMg86lJc?start=76&modestbranding=1&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> 1:16 | Duplicate one of the objects. |
</div>

---

:::{table} This is a **standard** _Markdown_ title
:align: center
:widths: grid


| Time Code | Description |
|-----------|-------------|
| <iframe width="400" height="226" src="https://www.youtube.com/embed/lFtEMg86lJc?start=74&modestbranding=1&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> 1:14 | Stop the simulation and go back to the beginning. |
| <iframe width="200" height="113" src="https://www.youtube.com/embed/lFtEMg86lJc?start=76&modestbranding=1&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> 1:16| Duplicate one of the objects. |
| <iframe width="200" height="113" src="https://www.youtube.com/embed/lFtEMg86lJc?start=77&modestbranding=1&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> | Optionally rotate the duplicated object. |
| <iframe width="200" height="113" src="https://www.youtube.com/embed/lFtEMg86lJc?start=89&modestbranding=1&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> | Press play and observe the stacked objects. |
| <iframe width="200" height="113" src="https://www.youtube.com/embed/lFtEMg86lJc?start=92&modestbranding=1&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> | Manipulate the stacked objects as desired. |
| <iframe width="200" height="113" src="https://www.youtube.com/embed/lFtEMg86lJc?start=98&modestbranding=1&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> | Simready assets come pre-packaged with these features. |
| <iframe width="200" height="113" src="https://www.youtube.com/embed/lFtEMg86lJc?start=103&modestbranding=1&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> | Simready assets are organized with a payload and a reference to the model. |
| <iframe width="200" height="113" src="https://www.youtube.com/embed/lFtEMg86lJc?start=114&modestbranding=1&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> | Inside, there is always one main transform, underneath which are the meshes. |
| <iframe width="200" height="113" src="https://www.youtube.com/embed/lFtEMg86lJc?start=120&modestbranding=0&rel=0" title="Simready video" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> | These meshes can be for rendering or collision detection. |
| <iframe width="200" height="113" src="https://www.youtube.com/embed/lFtEMg86lJc?

:::