# Shaders_Unreal
 A collection of shaders and material functions for Unreal Engine 4 and 5

 ## Unreal Material Functions

 ## Unreal ShaderFX

 ## Unreal Shaders for Postprocessing
 ### Outline Effect
 The outline effect is a basic effect which is based on the outline effect in Borderlands.
 How to use: Copy and paste PostProcess_Outline.uasset and PostProcess_Outline_Inst.uasset into your content folder. Inside the post processing volume, add a slot for a postprocessing material and select the PostProcess_Outline_Inst. To access the settings, open the material instance from the content browser.

 ### Sharpening Effect
 This effect mimics the High Pass overlay effect in Photoshop, which uses blurred high frequency details to accentuate details. In our case high frequency means the areas with the greatest contrast differences, which basically are most object edges and highest depth changes.
 How to use: Copy and paste PostProcess_Sharpening.uasset and PostProcess_Sharpening_Inst.uasset into your content folder. Inside the post processing volume, add a slot for a postprocessing material and select the PostProcess_Sharpening_Inst. To access the settings, open the material instance from the content browser.
