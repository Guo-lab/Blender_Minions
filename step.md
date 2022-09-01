# 3D character _ Minions

#### When it comes to the 3D character modeling, I start with Minions.

### Part 1: 

- New blender file and drop the reference picture into Blender.

- Put the front reference of the character in the front of the graphic view. Just like this: 

<img src="md_assets/image-20220830212141485.png" alt="image-20220830212141485" style="zoom:30%;" align='left' />

- ADD a cube to make the body. 
  Then, [Z] change into Wireframe. Choose the object, in Edit Mode, select the top vertices and change the shape. 
  Modifier Properties, ADD subdivision.  [Command R] to choose Edge Loop.
  Then, in Object Mode, smoothen the cube. 

- Back to Edit Mode after adjusting the position, (WireFrame could select just like X-ray in Solid View)

  <img src="md_assets/image-20220830214815453.png" alt="image-20220830214815453" style="zoom:30%;" />    <img src="md_assets/image-20220830223745881.png" alt="image-20220830223745881" style="zoom:21%;" />

  So, shape it.
  [Alt click] Select Edge Loop and Add-ons LoopTools to get Cycle.

  Choose half of the body and Use Mirror Modifier to make sure that it is symmetrical. (Mirror before Subdivision)

- Make the legs and feet: Press I to make faces. E to extrude and [SZ0] to falt the surface. Then, the arms. Get a little monster.

  <img src="md_assets/image-20220831003351287.png" alt="image-20220831003351287" style="zoom:30%;" />  <img src="md_assets/image-20220831014625191.png" alt="image-20220831014625191" style="zoom:40%;" />



- Make the gloves and shoes so on.    <img src="md_assets/image-20220831020753399.png" alt="image-20220831020753399" style="zoom:10%;" />    

- This is the first part.

   <img src="md_assets/image-20220831031213473.png" alt="image-20220831031213473" style="zoom:50%;" align='left' />



### Part 2:

- Get two lines on the head and Duplicate them as a **goggle**. 
  [P] to select them as single object.
  Create a mesh-Cycle, [RZ90] to place it vertically. 
  [EZZ] to extrude. [EescMedianPointS] to create top surface.
  Select the faces and [Alt E] can extrude faces along normals. (towards inside)

  - Create the button: 
    Select the Loop Faces. In select, Checker Deselect, [I] to insert faces and [altE to extrude faces along the normals outside]

  - Create the len of the goggles.
    [EescS] [EescS] [EescS] [F] (in order to later [GZZO] to extrude to the eye)
    Right Click set origin to geometry.

    [SshiftZ] Scale along the X axis.

  <img src="md_assets/image-20220831210454084.png" alt="image-20220831210454084" style="zoom:20%;" align='left'/>

- Create the **mouth** !
  Make a hole and ADD some details.

  <img src="md_assets/image-20220831212001066.png" alt="image-20220831212001066" style="zoom:30%;" align='left'/>              <img src="md_assets/image-20220831213004713.png" alt="image-20220831213004713" style="zoom:15%;" />

  ​              <img src="md_assets/image-20220831214001555.png" alt="image-20220831214001555" style="zoom:19%;" /> 



- Next, the teeth.
  [command J] to combine all teeth into onr object. Select UpTeeth and LowTeeth and click Control M and Z to choose the Mirror Axis. Last, give teeth one angle.
  <img src="md_assets/image-20220831220334753.png" alt="image-20220831220334753" style="zoom:20%;" />

- This is Part 2: 

  <img src="md_assets/image-20220831221307238.png" alt="image-20220831221307238" style="zoom:30%;"  align='left'/>

  

### Part 3: The Clothes.

- Front View, Edit Mode, Face Select, [C] to Cycle select. Like this.

  <img src="md_assets/image-20220901164609881.png" alt="image-20220901164609881" style="zoom:30%;" /> 

  And, esc to quit the Cycle Select mode.

- > After shift D to duplicate. Use P to select the object in the object mode.
  >
  > Solidify as next Modifier.

  Object mode, command A to Scale it.

  Mesh is so difficult! To invert them into triangles. (Pocket !)

  M to merge (eight (instead of six) edges to four)

  Ref:                                                                                        My:

  <img src="md_assets/image-20220901182741380.png" alt="image-20220901182741380" style="zoom:25%;" />    <img src="md_assets/image-20220901182645619.png" alt="image-20220901182645619" style="zoom:52%;" />

  So, ......

- **Screws**: UV Sphere. **Shoulder straps:** Plane and [E]

  Srews: 

  <img src="md_assets/image-20220901185412656.png" alt="image-20220901185412656" style="zoom:20%;" />   <img src="md_assets/image-20220901185450256.png" alt="image-20220901185450256" style="zoom:24%;" /> <img src="md_assets/image-20220901185529345.png" alt="image-20220901185529345" style="zoom:21%;" />   <img src="md_assets/image-20220901185916822.png" alt="image-20220901185916822" style="zoom:18%;" />

  Then, some details. Get this:

  <img src="md_assets/image-20220901192524467.png" alt="image-20220901192524467" style="zoom:50%;" /> 

- **Eyeball**:

   Shift H to isolate the transformed UV sphere. Biger duplicated UV Sphere could be the Up and Low.

  <img src="md_assets/image-20220901204620765.png" alt="image-20220901204620765" style="zoom:30%;" align='left'/>

- ---





### Part 4: Texturing

- Shade Editor:

  - Glass BSDF: 

    <img src="md_assets/image-20220901210612404.png" alt="image-20220901210612404" style="zoom:150%;" align='left'/><img src="md_assets/image-20220901210915488.png" alt="image-20220901210915488s" style="zoom:50%;" />

    <img src="md_assets/image-20220901211010842.png" alt="image-20220901211010842" style="zoom:40%;" align='left'/>

    **Transparent glasses.**

    Screen Space Refraction. ?

    

- UV editor:

  - Except Image Texture, Use Add-on Node Wrangler.
    Pricinpled BSDF and Ctrl T.

    <img src="md_assets/image-20220901212755382.png" alt="image-20220901212755382" style="zoom:50%;" />
  
  - How to use unwrap:
  
    Get a Edge Loop and [U] to mark the seam and [A] [U] to unwrap
  
  - Black and White Eyeball; Mix Shader
  
    OK, 
  
    <img src="md_assets/image-20220901223811062.png" alt="image-20220901223811062" style="zoom:34%;" /><img src="md_assets/image-20220901223843073.png" alt="image-20220901223843073" style="zoom:30%;" />

- Clothing and the Last Result :

  <img src="md_assets/res.png" alt="res" style="zoom:34%;" />

  
