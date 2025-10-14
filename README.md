<img width="240" height="840" alt="Screenshot 2025-10-14 225120" src="https://github.com/user-attachments/assets/12c719a0-5b9b-4ad4-b159-57d08f4a3d7e" /># MeshMaster
Mesh Master is a powerful Blender addon designed to streamline mesh cleanup, export, and turnaround rendering. It combines intelligent cleanup tools, batch export functionality, and automatic turnaround renders with dynamic lighting, all accessible from the Sidebar.

<img width="240" height="840" alt="Screenshot 2025-10-14 225120" src="https://github.com/user-attachments/assets/a1beec36-0854-41cf-8d86-9643e4e524a9" />

**Features**:

🧹 **Cleanup Tools**

Perform batch cleanup on selected mesh objects to improve mesh quality and consistency.

Merge By Distance: Merge vertices that are closer than a threshold.

Recalculate Normals: Make normals consistent.

Make Normals Outward: Ensure all normals face outward for correct shading.

Delete Loose Geometry: Remove isolated vertices, edges, or faces.

Fill Mesh Holes: Automatically fill small holes in the mesh.

Triangulate Faces: Convert all faces to triangles for cleaner topology.

Apply Transforms: Apply location, rotation, and scale transformations.

Select N-gons: Select all faces with more than 4 vertices.

📤**Export Tools**

Easily export meshes to FBX with options for modifiers, selection, and custom filenames.

Export Directory: Set where FBX files are saved.

Custom Filename: Optional custom name for exported files.

Apply Modifiers: Apply all object modifiers before export.

Selected Objects Only: Export only selected objects or all objects in the scene.

Export FBX Button: Quickly export with the selected settings.


🎥 **Turnaround Render**

Automatically generate multiple renders of your object rotating around its center with smart lighting.

Output Directory: Set where rendered images are saved.

Resolution: Set X and Y resolution for renders.

Number of Angles: Number of images around the object (360° divided by this number).

Image Format: PNG or JPEG.

Renderer: Cycles, Eevee, or Workbench.

Enable Clay Material: Replace object materials with a clay shader for consistent lighting.

Rim Light Color & Power: Customize lighting color and intensity for renders.

Render Turnaround Button: Automatically render multiple angles and clean up temporary lights/camera after rendering.


**Usage**:


Cleanup Meshes

Select one or more mesh objects.

Toggle desired cleanup options (e.g., Merge By Distance, Triangulate Faces).

Click Run Cleanup to apply.

Optionally, click Apply Transforms or Select N-gons for additional mesh preparation.

Export Meshes

Set the Export Directory.

(Optional) Add a Custom Filename.

Toggle Apply Modifiers and Selected Objects Only as needed.

Click Export FBX to save your mesh files.

Turnaround Rendering

Select the active object to render.

Set the Output Directory, Resolution, Number of Angles, and other render options.

Click Render Turnaround. The addon will automatically:

Position a temporary camera around the object.

Add temporary lights with specified colors and power.

Render all angles.

Delete temporary lights and camera after rendering.
