![Banner](banner.png)

# dso-image-metadata-remover
A command-line tool to remove potentially sensitive metadata (EXIF, IPTC, XMP) from image files. Uses Pillow library. - Focused on Tools for sanitizing and obfuscating sensitive data within text files and structured data formats

## Install
`git clone https://github.com/ShadowStrikeHQ/dso-image-metadata-remover`

## Usage
`./dso-image-metadata-remover [params]`

## Parameters
- `input_file`: The input image file
- `output_file`: The output image file (will overwrite if it exists). It must not be the input file itself. If the resolved output path is the same file as the input, whether spelled the same way, with a `./` prefix, or through a symlink, the run is refused with exit code 1 before anything is written, and the input file is left unchanged.
- `-h`: Show help message and exit
- `--keep-color-profile`: Preserve color profile

## License
Copyright (c) ShadowStrikeHQ
