# Keeping animated PNG iMessage stickers under 500KB

With the release of iOS 10, Apple introduced stickers in iMessage. A sticker
is a small image or animation that can be sent or placed on messages, photos
or on other stickers.

![iMessage panda sticker](/Screenshots/sticker-example-animated.gif?raw=true "iMessage panda sticker")

Creating a sticker pack with your own animated stickers is simple! You need an
**[animated PNG](https://en.wikipedia.org/wiki/APNG)** and
**[Xcode 8](https://developer.apple.com/xcode/)**.
Clone this project to get started, watch Apple's
[video tutorial](https://developer.apple.com/videos/play/tutorials/building-sticker-packs/),
or follow the steps below.

Keeping **animated stickers below the maximum size of 500KB** can be
challenging. We'll show you how you can use [TinyPNG](https://tinypng.com) to
accomplish this! **Read on!**

## Creating an iMessage Sticker Pack Application

First create a new Sticker Pack Application in Xcode 8. Select *File* > *New* >
*Project* from the menu, then choose *Sticker Pack Application*.

![Create new project, step 1](/Screenshots/new-project-1.png?raw=true "Create new project, step 1")

Name your project and choose a location to save it.

![Create new project, step 2](/Screenshots/new-project-2.png?raw=true "Create new project, step 2")

## Adding an animated PNG to your Sticker Pack

Your project is empty after creation. If you already have an animated PNG
(APNG), you can drag and drop it to the sticker pack under
*Stickers.xcstickers* > *Sticker Pack*.

![Empty project](/Screenshots/project-empty.png?raw=true "Empty project")

![Drag and drop sticker](/Screenshots/project-panda.png?raw=true "Drag and drop sticker")

For optimal performance, Apple has added a hard **file size limit of 500KB**
for stickers. Xcode will warn you when you attempt to add a file that is
larger.

![Error when over 500KB](/Screenshots/project-too-large.png?raw=true "Error when over 500KB")

Making sure your stickers are below 500KB can be especially challenging for
animated stickers! Luckily you can use [TinyPNG](https://tinypng.com) to
compress your stickers.

## Compressing animated PNGs

You can compress your images in order to reduce the file size. With the
TinyPNG website you can [compress APNG files](https://tinypng.com) for free.
This allows you squeeze every last byte out of your images and to create the
best possible stickers!

![APNG is now under 500KB](/Screenshots/tinypng-compression.png?raw=true "APNG is now under 500KB")

## Compare before & after

The compression uses advanced techniques to compress images. The difference is
hardly noticeable but the filesize savings after compression are quite
spectacular. The APNG image of the waving panda is compressed from 1.5 MB to
492 KB. You can see there is barely a visible difference.

**Note that animated PNGs are only displayed in Firefox or Safari. In Google
Chrome, Opera, Microsoft Edge and other browsers you only see the first
frame.**

Original APNG – 1.5MB | Optimised APNG – 492KB
----------------------------- | ------------------------------
![Original](/Source/panda-original.png?raw=true "Original") | ![Compressed](/StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/panda.sticker/panda.png?raw=true "Compressed")

## How to reduce file size further?

If [TinyPNG](https://tinypng.com) is not able to compress your animated PNG
below 500KB, you might have to take other steps to reduce the file size. You
may have to change your image so that the dimensions are smaller, or use fewer
frames.
