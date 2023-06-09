# img2irc (1.0.4)
![img2irc preview](https://i.imgur.com/oetHhMB.png)

img2irc is a utility which converts images to half or quarterblock irc/ansi art, with a lot of post-processing filters

*halfblock* means that each row will contain two rows worth of pixels, effectively doubling the vertical resolution

*quarterblock* (experimental) means that each row will contain two rows worth of pixels, and each column will contain two columns worth of pixels, quadrupling the resolution

the `irc` mode has 99 colours, the `ansi` mode has 256, `ansi24` has 16777216

## usage

`./img2ansi <URL or PATH> [OPTIONS]`

| option | description | default value |
| ------ | ----------- | ------------- |
| `<IMAGE>` | image url or file path | none |
| `--irc` | irc render type | true |
| `--ansi` | 8-bit ansi render type | false |
| `--ansi24` | 24-bit ansi render type | false |
| `--qb` | use quarterblocks | false |
| `-w, --width <WIDTH>` | output image width in columns | 50 |
| `-b, --brightness=<BRIGHTNESS>` | adjust brightness (-255 to 255) | 0 |
| `-c, --contrast=<CONTRAST>` | adjust contrast (-255 to 255) | 0 |
| `-s, --saturation=<SATURATION>` | adjust saturation (-255 to 255) | 0 |
| `-H, --hue <HUE>` | rotate hue (0 to 360) | 0 |
| `-g, --gamma <GAMMA>` | adjust gamma (0 to 255) | 0 |
| `--dither <DITHER>` | dithering (1 to 8) | 0 |
| `--pixelize <PIXELIZE>` | pixelize pixel size | 0 |
| `--gaussian-blur <GAUSSIAN_BLUR>` | gaussian blur radius | 0 |
| `--oil <OIL>` | oil ("[RADIUS],[INTENSITY]") | |
| `--grayscale` | converts image to black and white |
| `--nograyscale` | exclude grayscale colours from the palette |
| `--halftone` | made up of small dots creating a continuous-tone illusion |
| `--sepia` | brownish, aged appearance like old photographs |
| `--normalize` | adjusts brightness and contrast for better image quality |
| `--noise` | random variations in brightness and color like film grain |
| `--emboss` | gives a raised, 3d appearance |
| `--box-blur` | smoothed appearance like frosted glass |
| `--identity` | no modifications, unchanged image |
| `--laplace` | enhances edges and boundaries in an image |
| `--noise-reduction` | reduces noise for a cleaner, clearer image |
| `--sharpen` | increases clarity and definition, making edges and details more distinct |
| `--cali` | cool blue tone with increased contrast |
| `--dramatic` | high contrast and vivid colors for a dramatic effect |
| `--firenze` | warm, earthy tones reminiscent of tuscan landscapes |
| `--golden` | warm, golden glow like sunset light |
| `--lix` | high-contrast black and white appearance with increased sharpness |
| `--lofi` | low-fidelity, retro appearance like old photographs or film |
| `--neue` | clean, modern appearance with neutral colors and simple design |
| `--obsidian` | dark, monochromatic appearance with black and gray shades |
| `--pastel-pink` | soft, delicate pink tint like pastel colors |
| `--ryo` | bright, high-contrast appearance with vivid colors and sharp details |
| `--invert` | colors are inverted, opposite on the color wheel |
| `--frosted-glass` | blurred, frosted appearance as if viewed through semi-transparent surface |
| `--solarize` | strange, otherworldly appearance with inverted colors and surreal atmosphere |
| `--edge-detection` | highlights edges and boundaries in an image |
