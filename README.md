# Shaders_Unreal
 A collection of shaders and material functions for Unreal Engine 4 and 5

 ## Unreal Material Functions
 ### Material Function Collection
 This is a collection of basic and efficient material logic that can be used inside (master) materials in Unreal Engine 4 and 5. I do not maintain documentation on all functions as most of them are self explanatory. How to use: just drop them in a folder inside your project's content folder and they should be accessable.

 ## Unreal ShaderFX
 ### Object Outlines
 This effect is meant to highlight certain objects inside your gameworld. From the material instance you can change the color, gradients, line thicknes and distance fade.
 How to use: it's most efficient to create an object bp class and add the material from there. The material instance has a custom pass number, which has to be identical to the custom pass number on the mesh itself. Add a simple box as bounding box, overlapping the object and assign the material instance to this box. The box will be invisible and you should see the outline effect on the mesh it overlaps. This simple workflow makes sure the outline won't bleed onto other objects unintentionally.

![UnrealEditor_DaMTuPGtqj](https://github.com/bwvanlith/Shaders_Unreal/assets/47045108/c5a61455-f2c9-415e-a726-56f60808ff4d)

![UnrealEditor_YIHGIWcQDu](https://github.com/bwvanlith/Shaders_Unreal/assets/47045108/b0ca285a-c971-49c4-b4a9-f5219bdac0e9)

 ## Unreal Shaders for Postprocessing
 ### Outline Effect
 The outline effect is a basic effect which is based on the outline effect in Borderlands.
 How to use: Copy and paste PostProcess_Outline.uasset and PostProcess_Outline_Inst.uasset into your content folder. Inside the post processing volume, add a slot for a postprocessing material and select the PostProcess_Outline_Inst. To access the settings, open the material instance from the content browser.

 ### Sharpening Effect
 This effect mimics the High Pass overlay effect in Photoshop, which uses blurred high frequency details to accentuate details. In our case high frequency means the areas with the greatest contrast differences, which basically are most object edges and highest depth changes.
 How to use: Copy and paste PostProcess_Sharpening.uasset and PostProcess_Sharpening_Inst.uasset into your content folder. Inside the post processing volume, add a slot for a postprocessing material and select the PostProcess_Sharpening_Inst. To access the settings, open the material instance from the content browser.
