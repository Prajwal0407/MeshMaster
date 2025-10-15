# MeshMaster
Mesh Master is a powerful Blender addon designed to streamline mesh cleanup, export, and turnaround rendering. It combines intelligent cleanup tools, batch export functionality, and automatic turnaround renders with dynamic lighting, all accessible from the Sidebar.

<img width="245" height="987" alt="Screenshot 2025-10-15 065259" src="https://github.com/user-attachments/assets/2bb7d71b-94da-4ee4-abde-832de6b5d202" />


**🧠 Mesh Master — Ultimate Mesh Utility for Blender**

Author: Prajwal Mohite
Version: 1.0
Blender: 4.0+
Category: Object
Location: 3D Viewport → Sidebar → Mesh Master

**Overview**

Mesh Master is a powerful all-in-one Blender add-on for artists who need to prepare and export meshes quickly.
It combines essential utilities for:
Mesh cleanup
FBX export automation
Turnaround rendering with intelligent lighting
Origin (pivot) alignment tools
Ideal for asset preparation in game development, baking, or portfolio presentation.

**Installation**

1. Download the MeshMaster.py file.
2. In Blender, open Edit → Preferences → Add-ons → Install…
3. Select MeshMaster.py or MeshMaster.rar and click Install Add-on.
4. Enable Mesh Master in the Add-ons list.
5. Open the 3D Viewport, press N, and look for the Mesh Master tab.


Cleanup Tools

Perform common mesh optimization steps automatically.

| **Option**                | **Description**                                 |
| ------------------------- | ----------------------------------------------- |
| **Merge By Distance**     | Merge vertices that are close together.         |
| **Recalculate Normals**   | Make normals consistent across the mesh.        |
| **Make Normals Outward**  | Ensure all normals face outward.                |
| **Delete Loose Geometry** | Remove unconnected vertices, edges, or faces.   |
| **Fill Mesh Holes**       | Automatically fill small holes in the mesh.     |
| **Triangulate Faces**     | Convert all faces to triangles.                 |
| **Apply Transforms**      | Apply location, rotation, and scale transforms. |
| **Select N-gons**         | Select all faces with more than four sides.     |


Click Run Cleanup to execute all selected cleanup operations at once.

**📤 Export Tools**

Batch-export selected (or all) meshes as FBX with fine control.

| **Option**                | **Description**                                  |
| ------------------------- | ------------------------------------------------ |
| **Export Directory**      | Destination folder for exported FBX files.       |
| **Custom Filename**       | Optional override for object names.              |
| **Apply Modifiers**       | Apply modifiers before exporting.                |
| **Selected Objects Only** | Export only selected meshes or all in the scene. |


Press Export FBX to export meshes automatically.

**📍 Origin Tools**

Quickly change the pivot/origin of your mesh to precise bounding box positions.

| **Button**  | **Description**                        |
| ----------- | -------------------------------------- |
| **+X / -X** | Move origin to the right or left side. |
| **+Y / -Y** | Move origin to the front or back.      |
| **+Z / -Z** | Move origin to the top or bottom.      |
| **Center**  | Move origin to the center of the mesh. |


Useful for aligning pivots before exporting or animating.

**🎥 Turnaround Render**

Render a full 360° preview of your model with intelligent lighting setup.

| **Option**               | **Description**                                 |
| ------------------------ | ----------------------------------------------- |
| **Output Directory**     | Folder for rendered images.                     |
| **Resolution X / Y**     | Output render resolution.                       |
| **Image Format**         | Choose between PNG or JPEG.                     |
| **Renderer**             | Cycles, Eevee, or Workbench.                    |
| **Number of Angles**     | Number of renders per full rotation.            |
| **Enable Clay Material** | Use a neutral material for consistent lighting. |
| **Rim Light Color**      | Color of the rim light.                         |
| **Light Power**          | Intensity of the lighting setup.                |


Click Render Turnaround to automatically:
Create a temporary camera and lights.
Rotate around the object evenly.
Save all rendered frames to your selected directory.

**🧩 How It Works**

Mesh Master creates a property group (thegoodtools) that stores all your preferences per scene. Operators access these properties and perform Blender’s built-in mesh, export, and render operations in sequence — all from one easy UI.

**🧰 Technical Notes**

Works best in Object Mode when running cleanup or export tools.
Turnaround renders temporarily create and delete lights/camera after completion.
Exports use Blender’s native FBX exporter for compatibility.
Origin tools operate based on the object’s bounding box in world space.
