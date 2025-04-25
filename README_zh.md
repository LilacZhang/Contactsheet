# contactsheet
[English](README.md)

**contactsheet** 是一个基于 zsh 和 ImageMagick 的脚本，用于批量为照片添加黑色边框、压缩并生成拼接图。

## 功能

- 批量处理指定文件夹内的 JPG 图片，添加黑色边框并压缩至短边为1080p的图片。  
- 将处理后的图片按拼接图（Contact Sheet）的形式合并为单张 短边为1080p大小的图片。

## 预览

![Contactsheet](https://lilac-1315215436.cos.ap-guangzhou.myqcloud.com/img/202504251403978.jpg)

## 前提条件

- macOS 或 Linux 环境，支持 zsh。  
- 已安装 [ImageMagick](https://imagemagick.org/)。  
  ```sh
  brew install imagemagick        # macOS
  sudo apt install imagemagick    # Ubuntu / Debian
  ```

## 安装与使用

```sh
git clone https://github.com/<你的用户名>/contactsheet.git
cd contactsheet
chmod +x contactsheet

# 对指定文件夹运行脚本
./contactsheet /path/to/your/images
```

- 脚本执行完成后，会在目标文件夹中生成 `contactsheet.jpg` 并自动打开预览。  
- 临时生成的 `resized` 文件夹会在运行结束后自动删除。

## 示例

```sh
./contactsheet ~/Pictures/MyPhotos
```
## 其他
欢迎改进修改代码，提出请求即可。 
## 协议

本项目采用 MIT 许可证，详情请见 [LICENSE](LICENSE) 文件。