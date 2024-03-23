# Grab Text: A Screenshot to Clipboard Shell Script

This POSIX shell script triggers a screenshot tool to select an area, OCRs the content, and finally, copies the result to the clipboard.

<img src="logo.webp" alt="A sea shell looking through binoculars at text" width="300">

## Dependencies

[Tesseract OCR](https://github.com/tesseract-ocr/tesseract) is a _must-have_ without alternatives.

Supported Screenshot tools:

- [Make Image (maim)](https://github.com/naelstrof/maim)
- [SCReenshOT (scrot)](https://github.com/resurrecting-open-source-projects/scrot)
- [GNOME Screenshot (gnome-screenshot)](https://gitlab.gnome.org/GNOME/gnome-screenshot)
- [Shutter (shutter)](https://shutter-project.org/)

Supported Clipboard tools:

- [xsel](https://github.com/kfish/xsel)
- [xclip](https://github.com/astrand/xclip)

Optional tools:

- [Imagemagick (mogrify)](https://imagemagick.org/index.php) for optimizing the screenshot before OCR
- [libnotify (notify-send)](https://gitlab.gnome.org/GNOME/libnotify) for status notifications

## Installation

Download the script to any location in `$PATH` and `chmod +x`

With `curl`:

```shell
curl -L -o "$HOME/.local/bin/grab-text" https://raw.githubusercontent.com/benweidig/grab-text/main/grab-text
chmod +x "$HOME/.local/bin/grab-text"
```

With `wget`:

```shell
wget -O "$HOME/.local/bin/grab-text" https://raw.githubusercontent.com/benweidig/grab-text/main/grab-text
chmod +x "$HOME/.local/bin/grab-text"
```


## License

MIT. See [LICENSE](LICENSE)
