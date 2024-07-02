# [Image Viewer Application](https://github.com/li-jin-1998/Image-Viewer)

## Overview

The Image Viewer is a simple yet powerful desktop application built using Python and the PyQt5 framework. It allows
users to open, view, and interact with image files in various formats such as PNG, XPM, JPG,TIFF, and BMP. The
application features intuitive zooming capabilities, pixel value display, and custom background color adjustments based
on pixel values.

## Features

- **Open and View Images**: Users can open image files from their local filesystem and view them within the application.
- **Zoom In and Out**: The application supports zooming in and out using both the mouse wheel and keyboard shortcuts.
- **Fit to View**: Automatically scales the image to fit within the window while maintaining aspect ratio.
- **Pixel Value Display**: Displays the RGB values of the pixel under the mouse cursor.
- **Dynamic Background Color**: Changes the background color of the pixel value label based on the pixel's color,
  ensuring readability even with dark colors.
- **Save Last Open Path**: Remembers the last directory from which an image was opened, making it easier to navigate to
  commonly used folders.
- **Centered Window**: The application window is centered on the screen upon startup.
- **Keyboard Shortcuts**: Includes convenient keyboard shortcuts for opening files, zooming, resetting zoom, and closing
  the application.

## Installation

To install and run the Image Viewer application, follow these steps:

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/li-jin-1998/Image-Viewer.git
   cd Image-Viewer
   ```

2. **Install Dependencies**:
   Ensure you have Python installed, then install the required packages using pip:
   ```sh
   pip install PyQt5
   ```

3. **Run the Application**:
   ```sh
   python image_viewer.py
   ```

4. **PyInstaller Installation Guide:**
    ```
    pyinstaller --name ImageViewer --onefile --windowed image_viewer.py
    ```
    ```
    pip install -i https://pypi.tuna.tsinghua.edu.cn/simple opencv-python-headless
    pip install -i https://pypi.tuna.tsinghua.edu.cn/simple pyinstaller
    ```

    ```
    pyinstaller --clean ImageViewer.spec
    ```

## Usage

- **Open Image**: Press `Ctrl+O` or select "Open" from the "File" menu to open an image file.
- **Zoom In**: Press `Ctrl+=` or select "Zoom In" from the "View" menu to zoom into the image.
- **Zoom Out**: Press `Ctrl+-` or select "Zoom Out" from the "View" menu to zoom out of the image.
- **Reset Zoom**: Press `Ctrl+R` or select "Reset Zoom" from the "View" menu to reset the zoom level to fit the image
  within the window.
- **Close Application**: Press `Esc` to close the application.

## Code Structure

- **image_viewer.py**: Main application script containing the ImageViewer and GraphicsView classes.
- **ImageViewer.json**: Configuration file used to store the last open path.

## Customization

The application can be customized to add more features or modify existing ones. For instance, you can extend the
supported image formats, add image editing capabilities, or improve the user interface. The PyQt5 framework provides a
rich set of tools and widgets to enhance the functionality and aesthetics of the application.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a
pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
