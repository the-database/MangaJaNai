# MangaJaNai

[![Discord](https://img.shields.io/discord/1121653618173546546?label=Discord&logo=Discord&logoColor=white)](https://discord.gg/EeFfZUBvxj)

<a href="./mangajanaiv1demo.webp?raw=1"><img src="mangajanaiv1demo.webp"/></a>
<p align="center"><sup>(click image to enlarge)</sup></p>

## Overview

MangaJaNai is a collection of upscaling models for manga. The models are mainly optimized to upscale digital manga images of Japanese or English text with height ranging from around 1200px to 2048px.

Join the [**MangaJaNai Discord server**](https://discord.gg/EeFfZUBvxj) to get the latest news, download pre-release and experimental models, get support and ask questions, share your upscales, or share your feedback. 日本語も大丈夫です。

## Usage Instructions

### Upscaling with MangaJaNaiConverterGui

For a simple out of the box experience, use [MangaJaNaiConverterGui](https://github.com/the-database/MangaJaNaiConverterGui) to upscale your manga with the MangaJaNai models.

## MangaJaNai Models
While manga is produced at very high resolution (10000px+) and printed at excellent quality on physical book releases, official digital manga are often low resolution and riddled with JPEG and moiré artifacts. The aim of the MangaJaNai models is to upscale low quality black and white digital manga to produce results which clean up JPEG and moiré artifacts, delivering results that appear closer to the printed book versions. 

Most manga are produced with halftone dots, but some digital releases are so degraded that the halftone dots are no longer visible. The MangaJaNai models may appear to create dots that weren't in the original image, but in most cases the model correctly restores dots that were no longer visible in the low quality source image. In order to ensure that halftones are generated at the correct size and frequency, several MangaJaNai models were trained, each optimized to be used on images with one of seven different image heights, corresponding to the most common image sizes of digitally released manga in Japan: 1200p, 1300p, 1400p, 1500p, 1600p, 1920p, and 2048p. [MangaJaNaiConverterGui](https://github.com/the-database/MangaJaNaiConverterGui) automatically selects the best model to used depending on the resolution of the input image. 

## IllustrationJaNai Models
Since the MangaJaNai models are only suitable for black and white manga pages, supplementary IllustrationJaNai models were trained to be used for color images from manga, such as covers and color pages. These models were trained to remove common image artifacts, like JPEG artifacts and low resolution printed halftone dots. [MangaJaNaiConverterGui](https://github.com/the-database/MangaJaNaiConverterGui) automatically selects the IllustrationJaNai model for color images. 

## Related Projects

- [mpv-upscale-2x_animejanai](https://github.com/the-database/mpv-upscale-2x_animejanai): Real-time anime upscaling to 4k in mpv with Real-ESRGAN compact models
- [MangaJaNaiConverterGui](https://github.com/the-database/MangaJaNaiConverterGui): Windows GUI for manga upscaling with MangaJaNai models
