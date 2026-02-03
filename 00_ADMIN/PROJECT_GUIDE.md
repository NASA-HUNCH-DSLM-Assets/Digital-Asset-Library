# NASA HUNCH Digital Asset Project Guide

This guide provides the required workflow, documentation expectations, and technical standards for all teams contributing to the Digital Asset Library.

------------------------------------------------------------
1. Project Purpose
------------------------------------------------------------
High school teams collaborate to produce accurate 3D assets for NASA VR and AR simulations.  
These assets must be documented, organized, and stored in a consistent format.

------------------------------------------------------------
2. Required Tools
------------------------------------------------------------
Blender (free)
GitHub (version control and repository)
Git LFS (large file support)
Markdown (for documentation)
Image editor (for preview images)

------------------------------------------------------------
3. File Structure
------------------------------------------------------------
Each asset must be placed in its own folder:

Example:
CTB_3_0/
   CTB_3_0.fbx
   CTB_3_0.blend
   preview.png
   README.md
   textures/

Creative models follow the same layout.

------------------------------------------------------------
4. Documentation Requirements
------------------------------------------------------------
Each asset must include a README.md containing:

Asset Name  
Description  
Real-world dimensions (from Blender)  
File formats included  
Author and school  
Version number  
Notes on scale and orientation  
NASA specification reference (if required)  
Preview image  

------------------------------------------------------------
5. Technical Requirements
------------------------------------------------------------
- Models must be clean, manifold, and scaled in meters.
- Apply all transforms before export.
- Keep polycount reasonable unless otherwise required.
- Texture files must be included when applicable.
- Files must be exported in .fbx format.

------------------------------------------------------------
6. Contribution Process
------------------------------------------------------------
1. Fork the repository.
2. Create a new folder for your asset.
3. Add the model files and documentation.
4. Commit changes and push to your fork.
5. Submit a pull request to the main repository.
6. Wait for review feedback.
7. Make any required changes.
8. Once approved, your asset is merged.

------------------------------------------------------------
7. Quality Expectations
------------------------------------------------------------
- Required models must follow NASA dimensions exactly.
- Creative models must remain realistic, practical, and space-related.
- Documentation must be clear and complete.
- All assets must include preview images.
