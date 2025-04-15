# Bunkr Albums Enhanced - Infinite Scroll & Hover Previews

![Bunkr Albums Enhanced Preview](https://github.com/WendysBro/bunkr-albums-autoload-previews/raw/main/preview.gif)

## Features

- **Infinite Scroll**: Automatically loads more albums as you scroll down
- **Hover Previews**: See thumbnail previews when hovering over albums (200ms delay)
- **Multi-Domain Support**: Works with all Bunkr mirror domains (bunkr.si, bunkr.su, etc.)
- **Dual Page Support**: Works on both search results and top albums pages
- **Clickable Previews**: Click thumbnails to open full images/videos in new tab

## Installation

1. Install a userscript manager:
   - [Tampermonkey](https://www.tampermonkey.net/) (recommended)
   - [Violentmonkey](https://violentmonkey.github.io/)
   - [Greasemonkey](https://www.greasespot.net/)

2. Install the script:
   - [Direct install from GitHub](https://github.com/WendysBro/bunkr-albums-autoload-previews/raw/main/bunkr-albums-enhanced.user.js)
   - Or copy/paste the code into your manager

## Supported Pages

- Search results: `https://bunkr-albums.io/?search=*`
- Top albums: `https://bunkr-albums.io/topalbums*` (24h/7d/30d/all)

## Configuration

You can edit these values in the script:

```javascript
const CONFIG = {
    previewDelay: 200, // Hover delay in milliseconds
    maxPreviews: 15,   // Maximum thumbnails to show
    previewSize: '180px', // Thumbnail size
    scrollThreshold: 500 // Pixels from bottom to trigger load
};
```

## Troubleshooting

If the script isn't working:

1. Make sure you're using a supported userscript manager
2. Check the console for errors (F12 > Console)
3. Try disabling other Bunkr-related scripts
4. Open an [issue on GitHub](https://github.com/WendysBro/bunkr-albums-autoload-previews/issues)

## Development

Contributions welcome! Fork the repo and submit pull requests.

## License

MIT License - see [LICENSE](LICENSE) file
