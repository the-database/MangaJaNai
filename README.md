# MangaJaNai

[![Discord](https://img.shields.io/discord/1121653618173546546?label=Discord&logo=Discord&logoColor=white)](https://discord.gg/EeFfZUBvxj)

<a href="./demov3.webp?raw=1"><img src="mangajanaiv1demo.webp"/></a>
<p align="center"><sup>(click image to enlarge)</sup></p>

## Overview

MangaJaNai is a collection of upscaling models for manga. The models are mainly optimized to upscale digital manga images of Japanese or English text with height around 1200px.

Join the [**MangaJaNai Discord server**](https://discord.gg/EeFfZUBvxj) to get the latest news, download pre-release and experimental models, get support and ask questions, share your upscales, or share your feedback. 日本語も大丈夫です。

## Usage Instructions

### Upscaling with Chainner

1. Download and install [chaiNNer](https://chainner.app/download).
2. Download the .pth file of the model you would like to use for upscales.
3. Download [mangajanai pytorch.chn](mangajanai%20pytorch.chn?raw=1) file and open it in chaiNNer.
4. In the Load Model node, click on the text box below Pretrained Model to open a file dialog. Choose the .pth file that you downloaded in step 2.
5. In the Image File Iterator node, click on the text box below Base Directory and select the folder which contains the manga images you wish to upscale. All images must be extracted already, .cbz or .zip archives are not supported.
   1. If you wish to upscale a single chapter or volume of a manga then the folder you select should contain the images you want to upscale.
   2. If you wish to upscale an entire series which contains multiple volumes or chapters, then the folder you select should contain folders for each volume or chapter, where each of those folders contain the images you want to upscale.
6. In the Save Image node, click on the text box below Base Directory and select the folder where you want to save the upscales. Make sure this folder is different from the input folder you selected in the previous step so you don't overwrite your existing images.
7. Set your desired image quality settings in the Save Image node. WEBP format with 80 quality is suggested by default for good quality and efficient filesize compression, but the settings may be customize to suit your specific requirements.
8. Press the play button on the top bar in chaiNNer to begin upscaling.

### Upscaling with MangaJaNaiConverterGui

For a simpler out of the box experience, you can use the [MangaJaNaiConverterGui](https://github.com/the-database/MangaJaNaiConverterGui) program which includes the models and an interface built to make upscaling manga simple.

## Related Projects

- [mpv-upscale-2x_animejanai](https://github.com/the-database/mpv-upscale-2x_animejanai): Real-time anime upscaling to 4k in mpv with Real-ESRGAN compact models
- [MangaJaNaiConverterGui](https://github.com/the-database/MangaJaNaiConverterGui): Windows GUI for manga upscaling with MangaJaNai models
