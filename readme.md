# Awesome Image Tools [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools for compressing, converting, resizing, editing and inspecting images.

There are hundreds of image utilities and most "best image tool" lists are just affiliate roundups. This one is opinionated. It leans toward tools that **run in your browser without uploading your files**, tools that are **open source**, and the handful of hosted services that are genuinely worth the trade-off. Freemium tools are marked so you know before you click.

The list is intentionally small enough to maintain by hand. If a tool stops being free, changes its privacy model, or no longer deserves its spot, open an issue.

**Legend**

- 🔒 — Runs entirely in your browser. Files are never uploaded to a server.
- `OSS` — Open source. Source link in the entry.
- `$` — Has a paid tier. A usable free tier exists unless noted.

## Contents

- [Compression](#compression)
- [Format conversion](#format-conversion)
- [Resize & crop](#resize--crop)
- [Background removal](#background-removal)
- [Photo editors](#photo-editors)
- [Metadata & EXIF](#metadata--exif)
- [Passport & ID photos](#passport--id-photos)
- [Batch processing](#batch-processing)
- [SVG & vector](#svg--vector)
- [Favicons & app icons](#favicons--app-icons)
- [Color from images](#color-from-images)
- [Developer tools](#developer-tools)
- [Learn](#learn)
- [Contributing](#contributing)

## Compression

- [Caesium](https://saerasoft.com/caesium) `OSS` — Desktop compressor for Windows with a clear quality slider and side-by-side preview. Good for compressing a folder of photos in one pass.
- [Image Compressor](https://imagecompressor.com) 🔒 — Bulk JPG/PNG/WebP/GIF/SVG compression with a per-image quality slider, so you can push each one as far as it goes without visible artifacts.
- [ImageOptim](https://imageoptim.com) `OSS` — Mac drag-and-drop that strips junk metadata and runs several optimizers losslessly. The standard for shrinking images before they ship to a website.
- [imgkilo — compress to a target KB](https://imgkilo.com/compress-image-to-kb-size) 🔒 — Compress to a precise size like "under 100 KB", which is what government and job portals demand. Runs on the canvas in your tab.
- [Squoosh](https://squoosh.app) 🔒 `OSS` — The reference client-side compressor from the Chrome team. Live before/after slider, every modern codec via WebAssembly, and a real-time size readout. Start here.
- [TinyPNG](https://tinypng.com) `$` — Smart lossy compression for PNG, JPG and WebP. The free web drop handles 20 files at a time; the API is paid. Uploads to their servers.

## Format conversion

- [CloudConvert](https://cloudconvert.com) `$` — Converts between just about any image format and a lot of non-image ones too. Server-side, with an API and per-conversion pricing past the free quota.
- [Convertio](https://convertio.co) `$` — Broad format support with a simple drop-and-go flow. Free tier caps file size and daily conversions. Uploads required.
- [ImageMagick](https://imagemagick.org) `OSS` — The command-line workhorse. `convert in.heic out.jpg` and a thousand other things. If you script anything with images, you end up here.
- [imgkilo — HEIC to JPG](https://imgkilo.com/convert-heic-to-jpg-online) 🔒 — Turn iPhone HEIC photos into universal JPG without uploading them. Also covers WebP, AVIF, PNG and SVG conversions in the same place.
- [JXL Convert](https://jpegxlconvert.com) 🔒 `OSS` — Convert images to and from JPEG XL (.jxl), and HEIC to JPG/PNG, entirely in the browser with no upload; also opens and previews .jxl files.
- [Nutilz Image Converter](https://nutilz.com/image-converter) 🔒 — Converts JPG, PNG, WebP and BMP in the browser with a JPEG/WebP quality slider, before/after size comparison, and batch conversion to a ZIP. No upload.

## Resize & crop

- [Birme](https://www.birme.net) 🔒 — Bulk Resize Made Easy. Drop a folder, set one target size, drag each crop box, download a ZIP. All in the browser.
- [iLoveIMG](https://www.iloveimg.com/resize-image) `$` — A full hosted suite for resize, crop and compress. Convenient, but your images go to their servers; free tier has limits.
- [imgkilo — crop image](https://imgkilo.com/crop-image) 🔒 — Drag a box to crop to any aspect ratio or freeform, with a matching [circle crop](https://imgkilo.com/circle-crop) that exports a transparent PNG for avatars.
- [imgkilo — resize in pixels](https://imgkilo.com/resize-image-in-pixels) 🔒 — Set exact width and height (or fit within a maximum) with the aspect ratio locked, in the browser.

## Background removal

- [imgkilo — change photo background](https://imgkilo.com/change-photo-background) 🔒 — Cut out the subject and drop in white, a solid color, or transparency, in the browser. Handy for ID photos and simple product shots.
- [Photoroom](https://www.photoroom.com) `$` — Background removal aimed at product and marketplace photos, with templates and batch tools. Strong results; full resolution and batch need a plan.
- [rembg](https://github.com/danielgatis/rembg) `OSS` — Python library and CLI built on U²-Net. Self-host it to remove backgrounds in bulk with no per-image cost and nothing leaving your machine.
- [remove.bg](https://www.remove.bg) `$` — The service that made one-click cutouts mainstream. Excellent on hair and edges. Free downloads are low resolution; full-res and API are paid.

## Photo editors

- [ClearCrowds](https://www.clearcrowds.com) `$` — Hosted AI photo cleanup for removing crowds, objects, glare, shadows, text and other distractions from photos. Upload required; free trial path with paid limits.
- [GIMP](https://www.gimp.org) `OSS` — The long-standing free desktop alternative to Photoshop. Layers, masks, curves, scripting, the lot. Steep but complete.
- [Krita](https://krita.org) `OSS` — Open-source painting and illustration studio. Built for digital art and brushwork, but a capable raster editor in general.
- [Paint.NET](https://www.getpaint.net) — Free (closed source) Windows editor that sits between Paint and Photoshop. Layers and plugins without the GIMP learning curve.
- [Photopea](https://www.photopea.com) 🔒 `$` — Full-featured image editor in a browser tab. Opens and saves PSD, supports layers and adjustment layers, and keeps your files local. Free with ads.
- [Pixlr](https://pixlr.com) `$` — Browser editors (Pixlr X for quick edits, Pixlr E for advanced) with a familiar layout. Free tier is ad-supported.

## Metadata & EXIF

- [ExifTool](https://exiftool.org) `OSS` — Phil Harvey's command-line tool, the definitive way to read, write and strip metadata across every format and maker note that exists. The ground truth other tools are checked against.
- [imgkilo — EXIF viewer & remover](https://imgkilo.com/view-exif-data) 🔒 — Read the camera, date and GPS a photo carries, then [strip it](https://imgkilo.com/remove-exif-data) to a clean copy before sharing. Both run locally, which is the point when the data is your location.
- [Jeffrey's Image Metadata Viewer](http://exif.regex.info/) — A thorough online EXIF reader that surfaces fields most viewers skip, including a map for GPS tags. Uploads the file to read it, so use it on images you do not mind sharing.
- [Scrambled Exif](https://f-droid.org/packages/com.jarsilio.android.scrambledeggsif/) `OSS` — Android app that strips metadata from photos straight in the system share sheet, before they go to a chat or post.

## Passport & ID photos

- [IDPhotoDIY](https://www.idphotodiy.com) — Free browser tool with a large library of country and visa sizes, and a printable sheet layout. Dated UI, but it works and asks for nothing.
- [imgkilo — passport photo maker](https://imgkilo.com/passport-photo-maker) 🔒 — Remove or whiten the background, crop to a country or exam spec, and frame the head correctly, in the browser. Includes US [2×2](https://imgkilo.com/passport-photo-2x2) and many exam presets.
- [Passport Photo Maker (passports.pics)](https://passportphoto.passports.pics) 🔒 — Crop a photo to one of eight country and visa presets (US, UK, Schengen, India, China, Canada, Australia) with a head-size guide and a background check, then download the file and a 4×6 print sheet at 300 dpi, in the browser. You place the crop yourself; there is no automatic face detection.
- [Quick Image Kit — passport photo upload compressor](https://quickimagekit.com/compress-photo-for-passport-upload) 🔒 — Compress passport-style upload photos locally for forms with file-size limits.

## Batch processing

- [imgkilo — bulk compressor & converter](https://imgkilo.com/bulk-image-compressor) 🔒 — Drop a whole folder to compress, [convert](https://imgkilo.com/bulk-image-converter) or [resize](https://imgkilo.com/resize-multiple-images) every file at once and get a ZIP back, without uploading the batch.
- [ImageMagick `mogrify`](https://imagemagick.org/script/mogrify.php) `OSS` — Batch-edits images in place from one command: resize, convert, strip, or apply an effect to a whole directory.
- [XnConvert](https://www.xnview.com/en/xnconvert/) — Free desktop batch processor: queue hundreds of files, chain multiple actions, and save the recipe to reuse. Handy when the same transform runs every week.

## SVG & vector

- [imgkilo — SVG to PNG](https://imgkilo.com/convert-svg-to-png-online) 🔒 — Rasterize a vector SVG to a PNG at any pixel size you choose, in the browser.
- [SVGO](https://github.com/svg/svgo) `OSS` — The Node-based SVG optimizer. Strips editor cruft and shrinks files, scriptable and pluggable, the engine most other SVG optimizers wrap.
- [SVGOMG](https://jakearchibald.github.io/svgomg/) 🔒 `OSS` — Jake Archibald's GUI for SVGO. Toggle each optimization with a live preview and size readout. Entirely client-side.
- [Vectorizer.ai](https://vectorizer.ai) `$` — Traces a raster image (logo, sketch) into a clean SVG with surprisingly good results. Free preview, paid full-resolution downloads.

## Favicons & app icons

- [favicon.io](https://favicon.io) — Generates a favicon from text, an emoji, or an uploaded image. Fast and free for the common case.
- [RealFaviconGenerator](https://realfavicongenerator.net) — Produces the full set of icons and the markup for every platform, and checks how they render across browsers and devices. The thorough option.

## Color from images

- [Adobe Color](https://color.adobe.com/create/image) — Extract a color theme from any photo and tweak the harmony rules. Free with an Adobe account.
- [Coolors](https://coolors.co/image-picker) `$` — Generate a palette from an uploaded image and lock the colors you like. Free to use; pro unlocks extras.
- [Image Color Picker](https://imagecolorpicker.com) — Upload an image and click anywhere to read the exact hex, RGB and HSL. The quickest "what color is that pixel" tool.

## Developer tools

- [Image2Base64](https://image2base64.com/) 🔒 — Convert PNG, JPG, GIF, WebP, SVG, BMP and ICO images to Base64 data URIs and ready-to-paste HTML/CSS snippets entirely in the browser.
- [imgproxy](https://imgproxy.net) `OSS` `$` — A fast, secure standalone server for resizing and converting images on the fly behind a URL. Open-source core with a paid Pro tier.
- [libvips](https://www.libvips.org) `OSS` — A low-memory, high-speed image processing library. The engine under sharp and many CMS thumbnailers; reaches for it directly when throughput matters.
- [Pillow](https://pillow.readthedocs.io/) `OSS` — The Python imaging library. The default for scripting image work in Python: open, transform, save, automate.
- [sharp](https://sharp.pixelplumbing.com) `OSS` — The go-to Node.js image library, built on libvips. Fast resize, convert and composite for build pipelines and servers.
- [Thumbor](https://www.thumbor.org) `OSS` — An open-source imaging server with smart cropping that detects faces and points of interest to keep the subject in frame.

## Learn

- [An image format for the Web: WebP](https://developers.google.com/speed/webp) — Google's documentation on WebP, including how its lossy and lossless modes compare to JPG and PNG.
- [EXIF](https://en.wikipedia.org/wiki/Exif) — What the metadata block in a photo actually contains, including the GPS fields worth stripping before you share.
- [Image file type and format guide (MDN)](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types) — A clear reference on JPG, PNG, WebP, AVIF, SVG and GIF, and when to use each.
- [Learn Images (web.dev)](https://web.dev/learn/images/) — A full course on choosing formats, sizing, and serving images well on the web.

## Contributing

Suggestions and pull requests are welcome. Please read the [contribution guidelines](contributing.md) first — there is a short bar for what gets added, so the list stays useful rather than exhaustive.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this work. See [license](license).
