# Unity-Python RGBD Simulator

This package provide the ability to capture Unity's `PerceptionCamera` RGB and
depth image, and publish it to a Python endpoint via UDP for image processing.

> ⚠️ ***Please read the setup instructions carefully!***

## Setup Instructions

### 1. Install Unity High Definition Render Pipeline (HDRP)

Pick one of the following options:

![](/images/pacman.gif)
*Option 1: Importing Unity HDRP to existing projects*

![](/images/newproj.gif)
*Option 2: Creating new project with HDRP preinstalled*

### 2. Convert render materials to HDRP materials

This is necessary for `PerceptionCamera` to be able to see GameObjects. If there
is any `Fix All` option, select it. All checkmarks should be green on this
window.

![](/images/convert_materials.gif)
*Converting all project materials to HDRP compliant*

### 3. (Optional) Create and assign new materials as necessary

If your robots and objects does not render correctly i.e., it looks purple, it
means the shader for that material is wrong. The correct shader material needs
to be `HDRP/Lit`.

![](/images/create_material.gif)
*Creating new material and assign correct shader*

### 4. Install Unity Perception package

Add package via Unity package naming convention i.e., **`com.unity.perception`**

![](/images/import_perception.gif)
*Importing Unity Perception via Package Manager*

### 5. Import Unity-Python RGBD Capture Package

In this repository, the file
[CameraStreamer.unitypackage](./CameraStreamer.unitypackage) contains all the
necessary code and prefabs necessary to complete assignments. To import, go to
`Assets -> Import Package -> Custom Packages...`, which will open a file
selection dialog. Navigate to where you download the `.unitypackage` and select
it.

### 6. Add camera into scene

### 7. Verify Python communication