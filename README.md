# contactsheet
[中文](README_zh.md)

**contactsheet** is a zsh + ImageMagick script for batch‑adding a black border to photos, resizing them, and generating a contact sheet.

## Features

- Batch‑process all JPG images in a specified folder: add a black border and resize to fit within ×1080px.  
- Stitch the processed images into a single ×1080px contact sheet.

## Preview
![Contactsheet](fig/contactsheet.jpg)

## Requirements

- macOS or Linux with zsh.  
- [ImageMagick](https://imagemagick.org/) installed.  
  ```sh
  brew install imagemagick        # macOS
  sudo apt install imagemagick    # Ubuntu / Debian
  ```

## Installation & Usage

```sh
git clone https://github.com/<your-username>/contactsheet.git
cd contactsheet
chmod +x contactsheet

# Run the script on your target folder
./contactsheet /path/to/your/images
```

- When finished, `contactsheet.jpg` will appear in the target folder and open automatically.  
- The temporary `resized` folder is removed after execution.

## Example

```sh
./contactsheet ~/Pictures/MyPhotos
```

## Contributing

Feel free to suggest improvements or submit a pull request.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## Chinese Version

For the Chinese version, please refer to [README_zh.md](README_zh.md).  