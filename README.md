# SVG to PNG Bulk Converter for macOS

A simple, efficient, and free script for macOS users that enables batch conversion of SVG files to PNG format, leveraging native macOS tools. Eliminate the need for online converters with restrictions and effortlessly transform your SVGs into high-resolution PNGs straight from your terminal.

## Prerequisites

- A macOS machine
- Terminal access
- A folder containing SVG files you want to convert

## Usage

1. **Prepare Your Files:** 
    - Place all the SVG files you want to convert in a single folder.
  
2. **Navigate to the Folder:** 
    - Open your terminal and navigate to the directory containing the SVG files. You can use the `cd` command to change directories.
    ```
    cd path/to/your/folder/
    ```

3. **Run the Conversion Script:** 
    - Copy and paste the following command into your terminal and press `Enter`:
    ```bash
    for file in *.svg; do
        qlmanage -t -s 2000 -o . "$file"
    done
    ```
    - This script will convert all SVG files in the folder to PNG files with a width of 2000px. 

4. **Customize the Output Resolution:** 
    - To adjust the width of the output PNGs, modify the `2000` value in the `-s 2000` segment of the command. Replace `2000` with your desired width in pixels.

## Why Use This Script?

- **No More Online Limitations:** Skip the hassle of uploading files to online platforms, avoid size restrictions, and ensure your files remain private.
- **High-Quality Conversions:** Achieve excellent resolution PNGs tailored to your needs.
- **Quick and Efficient:** Especially beneficial when dealing with a large number of SVGs.

## Contributing

If you have suggestions for improving this script or find any issues, please open an issue or submit a pull request.

## License

This project is released under the GNU General Public License v3.0.
