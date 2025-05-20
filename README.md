# Blender Projects
Project files and images of the objects I created in Blender.

<br>

## Paintball

I designed this paintball gun as part of the [Paintball Polygon](https://github.com/elifnazlib/PaintballPolygon) project, with reference to [this model](https://sketchfab.com/3d-models/paintball-gun-c9f3b8079102454fb9d3fc628ff0ad8b).

<img src="https://github.com/elifnazlib/BlenderProjects/blob/main/Paintball/paintball.gif" width="515" />

<br>

<br>

> [!NOTE]
> When I exported the model as .fbx file and imported it to the Unity scene, some parts of the model seemed transparent. The problem was that if the model's face normals are pointing inward (flipped normals), Unity will cull (hide) the back side. To fix it in Blender:
> - Select the model
> - Then press Tab to go into Edit Mode
> - Then press A to select all
> - Finally press Alt + N --> choose Recalculate Outside
>
> Eventually, this will orient all normals to point outward.

<br>

> [!IMPORTANT]  
> In order to make the model appear with its material in Unity scene, you need to:
> - Export the model from Blender in .fbx format with Path Mode: Copy and check "Embed Textures" on the right side.
>   
>   <img width="182" alt="instruction1" src="https://github.com/user-attachments/assets/cb842fcb-b5f7-4b67-bf79-acb75f20a2aa" />
> - When imported into Unity, you can create a new material and set its shader to "Standard". Then, you can drag the texture image (gun color) into the Albedo slot.
>   
>   <img width="331" alt="material" src="https://github.com/user-attachments/assets/b7498ee0-834a-44af-af4c-50d60167741d" />
> - Then, assign this material as your model's.
> 
>  Now, you can see the model with its texture.
