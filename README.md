# NTU Racing Team KiCad Files

## Guide for configuring path variables and libraries

> [!NOTE]
> Before you start, please include the appropriate libraries and path variables to ensure components and their resources can be loaded correctly!

### 1. Configuring path variable

![image](https://github.com/user-attachments/assets/24e89efb-7beb-4a44-bff8-5997ec050622)\
![image](https://github.com/user-attachments/assets/ee9ea6a5-3d50-4d55-8bd4-2e3982e36277)

### 2. Configuring libraries
> [!NOTE]
> Configure symbol libraries and footprint libraries according to the README files located in each generation's directory. Images shown here are only for demonstration purposes only.

![image](https://github.com/user-attachments/assets/8d61c2a1-a55e-4454-b3c4-e93e2027c5b8)

## Adding 3D models
<img width="860" height="700" alt="image" src="https://github.com/user-attachments/assets/a339f3c2-e1dc-42ce-81a0-6a0728c5c67f" />

1. Copy the .step/.wrl files to `EPx/Libraries/3d_models` folder
2. In the footprint editor (press Ctrl+E on a footprint in the PCB editor), open footprint properties, navigate to the 3D Models tab, and select the 3D model file with the folder icon to the left of the Show checkbox.
3. The path should be replaced with `${NTURT_KICAD_ROOT}/EPx/Libraries/3d_models/...`, if not, then you will need to set up the path variable.
4. Adjust the position of the model.
> [!NOTE]
> For a part that a 3D model would be helpful, if it is a part that came with KiCad, then consider "Save as" in the footprint editor to the project library, then edit the 3D model.\
> If it is already from a project library, remember to select "Open in library XXX" if it says "Editing XXX from board." on top. After you're done, right click the footprint in the PCB editor and select Update Footprint, check Update/reset 3D models.
