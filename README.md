# PixelPruner
PixelPruner is a user-friendly image cropping app for AI-generated art. It supports PNG, JPG, JPEG, and WEBP formats. Easily crop, preview, and manage images with interactive previews, thumbnail views, rotation tools, and customizable output folders. Streamline your workflow and achieve perfect crops every time with PixelPruner.

  ![image](https://github.com/theallyprompts/PixelPruner/assets/133992794/bf264a2a-1192-428b-9c73-7da4b17d7313)
 
---

# Features
- **Multi-Format Support**: Supports cropping images in PNG, JPG, JPEG, and WEBP formats. Crops are converted to PNG.

- **Interactive Crop Previews**: Preview your crop selection in real-time with an interactive preview pane, before you make the crop.

  ![image](https://github.com/theallyprompts/PixelPruner/assets/133992794/5768c2f2-7573-4700-a79d-b38508ac9307)

- **Thumbnail View of Crops**: View all your cropped images as thumbnails in a dedicated pane, making it easy to manage and review your work.

  ![image](https://github.com/theallyprompts/PixelPruner/assets/133992794/e96b3dbb-924e-41b6-bf9f-46d581f3fcde)

- **Rotation Tools**: Easily rotate images to achieve the perfect orientation before cropping.

  ![image](https://github.com/theallyprompts/PixelPruner/assets/133992794/c1df184c-9aa5-4af5-bca9-c45cf40c24e4)

- **Multi-Crops**: Make multiple crops from the same image. Multiple faces? No problem!

  ![image](https://github.com/theallyprompts/PixelPruner/assets/133992794/9dac7fdb-6bb8-4c46-a863-9506701b219a)

- **Customizable Output Folder**: Choose a custom folder to save your cropped images.

- **Zip Crops**: Quickly zip all cropped images into a single archive for easy sharing, storage, or upload to the Civitai.com on-site LoRA Trainer

  ![image](https://github.com/theallyprompts/PixelPruner/assets/133992794/2c02c817-80ce-4280-8eca-2e6a198425e4)

- **Undo Crop Actions**: Made a mistake? Simply undo the last crop with the click of a button.

- **Keyboard Shortcuts**: Navigate and manipulate images effortlessly with convenient WASD keyboard shortcuts.

  ---

## Installation Guide - Prebuilt App

Head to the **[Releases](https://github.com/theallyprompts/PixelPruner/releases)** and download the latest .exe version - pre-packaged with Python and ready to run (no installation required!)

---

## Installation Guide - Manual Install

Follow these steps to install and run PixelPruner on your local machine.

### Prerequisites

1. **Python 3.x**: Make sure you have Python 3.x installed on your system. You can download it from the [official Python website](https://www.python.org/downloads/).

2. **Pillow**: This library is required for image processing. You can install it with the `pip` package manager.

### Step-by-Step Installation

1. **Clone the Repository**

   Clone the PixelPruner repository from GitHub to your local machine using the following command:

   ```sh
   git clone https://github.com/Davidss2/PixelPrunerLinux.git
   ```

2. **Navigate to the cloned directory**

3. **Set Up a Virtual Environment (Optional but Recommended)**

   It is recommended to use a virtual environment to manage dependencies. Create and activate a virtual environment:

   ```sh
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   ```

4. **Install Dependencies**

    Install the required dependencies using pip:

    ```sh
    pip install pillow[webp]
    pip install tkinterdnd2
    ```

    If you're on Linux, you might need to install tkinter separately:

    ```sh
    sudo apt-get install python3-tk
    ```

5. **Running the Application**

    Run the PixelPruner application using the following command: 

    ```sh
    python PixelPruner.py
    ```

---

### Using PixelPruner

**Select Folder**: After launching the app, you can either drag a set of images into the main pane, or go to `File > Set Input Folder`, to select a folder of input images.

**Select Crop Dimensions**: From the dropdown in the top left, select the output dimensions for your crops.

**Set an output Directory** (optional): Click `File > Set Output Directory` to choose a folder to save your crops. If no directory is chosen, PixelPruner will place crops beside the original images. Note: if you've dragged images into PixelPruner, you must manually set an output directory.

**Crop and Manage Images**: Use the interactive tools to crop, rotate, and manage your images. Cropped images can be previewed and saved to a custom output folder.

**Keyboard Shortcuts**: Use keyboard shortcuts (W, S) to navigate through images and (A, D) to rotate them. Ctrl+Z will undo the last crop.

---

### Roadmap

1. ~~**Add a toggle for advance-on-crop**: Why on earth did I add an auto-advance on crop? What a huge mistake! The next update will add a toggle to choose whether to advance-on-crop or remain on the current image.~~ Completed in v1.1.0

2. ~~Input and Output Folder selection improvements - I want to be able to switch input directory mid cropping-session!~~ Completed in v1.2.0

3. ~~**More Options for Input** - Ability to drag a selection of images into the app for cropping, rather than select from a folder. That sounds useful.~~ Completed in v2.0.0

4. ~~**A Better Menu** - A proper file menu system.~~ Added in v2.0.0

5. **User Settings** - The ability to save user preferences.

6. **Simple image editing** - brightness, contrast, sharpness, etc. I want to be able to do as much as possible as easily as possible, without having to photoshop anything prior to upload to Civitai.

7. **API Access to Civitai.com's LoRA Trainer**: Upload zipped crops directly into Civitai.com's on-site LoRA trainer. The API for this doesn't exist yet, but maybe if I ask nicely...

---

### Created By...

**[TheAlly](https://civitai.com/user/theally)** - A coding amateur with zero application development experience. I threw this together with the help of **ChatGPT 4o** because I couldn't find a tool which offered the features I required in a cropping/data set prep tool for LoRA Training.
