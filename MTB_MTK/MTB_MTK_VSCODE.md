
# μT-Kernel 3.0 BSP2 Setup for Infineon Modustoolbox-VSCode

## Step by Step Example

### Prerequisites
- [μT-Kernel 3.0 BSP2](https://www.tron.org/ja/page-6100/)
- [μT-Kernel 3.0 BSP2 for ModusToolBox](https://github.com/tron-forum/mtk3_bsp2/blob/main/doc/bsp2_xmc_mtb_jp.md/)
- [Infineon Modustoolbox](https://www.infineon.com/cms/en/design-support/tools/sdk/modustoolbox-software/)
- [VS Code](https://code.visualstudio.com/)
- [Kit XMC72 EVK](https://www.infineon.com/cms/en/product/evaluation-boards/kit_xmc72_evk/)

### Setup Instructions

1. **Open ModusToolBox 3.2 Dashboard**
   - Create a new application (workspace)
   ![alt text](/MTB_MTK/images/image.png)
   - Set the workspace path
   ![alt text](/MTB_MTK/images/image-1.png)
   - Create a new application
   ![alt text](/MTB_MTK/images/image-2.png)
   - Choose the target device
   ![alt text](/MTB_MTK/images/image-3.png)
   - Choose example code and set the project name
   ![alt text](/MTB_MTK/images/image-4.png)
   - Wait for the project to be created (2 projects will be created: `0000_mtk_project` and `mtk_share`)
   ![alt text](/MTB_MTK/images/image-5.png)

2. **Clone the μT-Kernel 3.0 BSP2 Files**
   - Open a terminal
   - Navigate to the project path
   ![alt text](/MTB_MTK/images/image-6.png)
   - Clone the μT-Kernel 3.0 BSP2 files using:
     ```bash
     git clone --recursive  https://github.com/tron-forum/mtk3_bsp2.git
     ```
     ![alt text](/MTB_MTK/images/image-7.png)
   - Verify that the `mtk3_bsp2` folder has been created

3. **Edit Project Files**
   - Edit the `Makefile` as required
   ![alt text](/MTB_MTK/images/image-8.png)
   - Edit `main.c` to include necessary changes
   ![alt text](/MTB_MTK/images/image-9.png)

4. **Create User Application**
   - Create a user application folder
   ![alt text](/MTB_MTK/images/image-10.png)
   - Create the user application file in the newly created folder
   ![alt text](/MTB_MTK/images/image-11.png)
   - Edit the application [source file](https://github.com/tron-forum/mtk3_bsp2/blob/main/doc/bsp2_xmc_mtb_jp.md#433-%E3%83%97%E3%83%AD%E3%82%B0%E3%83%A9%E3%83%A0%E4%BE%8B)
   ![alt text](/MTB_MTK/images/image-12.png)

5. **Build the Project**
   - Build the project
   ![alt text](/MTB_MTK/images/image-13.png)
   - Ensure the build finishes successfully
   ![alt text](/MTB_MTK/images/image-14.png)

6. **Program the Device**
   - Open the programmer
   ![alt text](/MTB_MTK/images/image-15.png)
   - Skip the KitProg update if prompted
   ![alt text](/MTB_MTK/images/image-16.png)
   - Connect the device and ensure the correct file path is selected
   ![alt text](/MTB_MTK/images/image-17.png)
   - Program the device and check the output on the UART
   ![alt text](/MTB_MTK/images/image-18.png)
   ![alt text](/MTB_MTK/images/image-19.png)

7. **Transfer the Project to VSCode**
   - **Why?** For code auto-completion and AI code suggestions
   ![alt text](/MTB_MTK/images/image-20.png)
   - Generate the VSCode files from ModusToolbox
   ![alt text](/MTB_MTK/images/image-21.png)
   ![alt text](/MTB_MTK/images/image-22.png)
   - Open the generated files in VSCode
   ![alt text](/MTB_MTK/images/image-23.png)
   - Trust the project when prompted
   ![alt text](/MTB_MTK/images/image-24.png)
   - Install necessary plugins in VSCode
   ![alt text](/MTB_MTK/images/image-25.png)

8. **Edit and Build in VSCode**
   - Edit `app_main.c` in VSCode
   ![alt text](/MTB_MTK/images/image-26.png)
   - Build the project in VSCode
   ![alt text](/MTB_MTK/images/image-27.png)
   - Ensure the build finishes successfully
   ![alt text](/MTB_MTK/images/image-28.png)

9. **Program the Device from VSCode**
   - Open the programmer
   ![alt text](/MTB_MTK/images/image-29.png)
   - Skip the KitProg update if prompted
   ![alt text](/MTB_MTK/images/image-30.png)
   - Connect the device and ensure the correct file path is selected
   ![alt text](/MTB_MTK/images/image-31.png)
   - Program the device and check the output on the UART
   ![alt text](/MTB_MTK/images/image-32.png)
   ![alt text](/MTB_MTK/images/image-33.png)

### Additional Tips
- Make sure to frequently save your work and commit changes to version control
- Refer to official documentation for troubleshooting and advanced configurations

### Reference Links
- [Infineon Modustoolbox](https://www.infineon.com/cms/en/design-support/tools/sdk/modustoolbox-software/)
- [VS Code](https://code.visualstudio.com/)
- [Kit XMC72 EVK](https://www.infineon.com/cms/en/product/evaluation-boards/kit_xmc72_evk/)

### Contact:
- wjbthu@gmail.com

