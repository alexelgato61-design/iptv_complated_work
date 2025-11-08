# IPTV Player - Localhost Edition

A simple, web-based IPTV player that works perfectly on localhost. Stream your favorite channels with an elegant and user-friendly interface.

## Features

- 📺 Clean and modern web interface
- 🎬 Supports multiple stream formats (M3U8, MP4, and more)
- 📋 Built-in playlist support (M3U format)
- 🚀 Easy to run - just open in a browser
- 📱 Responsive design - works on desktop and mobile
- ⚡ No installation required - pure HTML, CSS, and JavaScript

## Quick Start

### Method 1: Simple File Opening (Basic)
1. Clone this repository or download the files
2. Open `index.html` in your web browser
3. Start streaming!

### Method 2: Local HTTP Server (Recommended)

For better compatibility and to avoid CORS issues, run a local HTTP server:

#### Using Python 3:
```bash
python -m http.server 8000
```

#### Using Python 2:
```bash
python -m SimpleHTTPServer 8000
```

#### Using Node.js (http-server):
```bash
npx http-server -p 8000
```

#### Using PHP:
```bash
php -S localhost:8000
```

Then open your browser and navigate to:
```
http://localhost:8000
```

## Usage

### Playing Channels from the Playlist

1. Click on any channel from the "Sample Channels" list on the right
2. The video player will automatically load and play the stream

### Loading a Custom Stream

1. Enter a stream URL in the input field (supports M3U8, MP4, etc.)
2. Click the "Load" button or press Enter
3. The stream will start playing in the video player

### Using Your Own Playlist

1. Create a `.m3u` file with your channels (see format below)
2. Replace or edit the `playlist.m3u` file
3. Click "Load Playlist" to refresh the channel list

## M3U Playlist Format

The playlist uses the standard M3U format:

```m3u
#EXTM3U
#EXTINF:-1,Channel Name 1
http://example.com/stream1.m3u8
#EXTINF:-1,Channel Name 2
http://example.com/stream2.m3u8
```

## Supported Stream Formats

- HLS (HTTP Live Streaming) - `.m3u8`
- MP4 - `.mp4`
- WebM - `.webm`
- OGG - `.ogg`
- Any format supported by HTML5 video element

## Project Structure

```
iptv_complated_work/
│
├── index.html          # Main IPTV player interface
├── playlist.m3u        # Sample playlist with test streams
├── README.md           # This file
└── .gitignore         # Git ignore file
```

## Troubleshooting

### Video not playing?
- Check if the stream URL is valid and accessible
- Some streams may have CORS restrictions - use a local HTTP server
- Ensure your browser supports the stream format
- Check browser console for error messages

### Playlist not loading?
- Make sure `playlist.m3u` is in the same directory as `index.html`
- If opening `index.html` directly, the playlist may not load due to browser security restrictions
- Solution: Run a local HTTP server (see Quick Start)

### Browser Compatibility
The player works best with modern browsers:
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

## Adding Your Own Streams

1. Edit `playlist.m3u` to add your stream URLs
2. Use the format:
   ```
   #EXTINF:-1,Your Channel Name
   http://your-stream-url.com/stream.m3u8
   ```
3. Reload the page and click "Load Playlist"

Or simply paste any stream URL directly into the input field!

## Technologies Used

- HTML5 Video API
- CSS3 (Grid, Flexbox, Gradients)
- Vanilla JavaScript (No dependencies!)
- M3U Playlist Parser

## License

This project is open source and available for personal and educational use.

## Notes

- The sample streams included are public test streams
- For production use, ensure you have rights to stream the content
- This is a client-side player - streams must be publicly accessible

## Contributing

Feel free to fork this project and add your own features:
- Volume controls
- Fullscreen mode enhancements
- More playlist formats
- Stream quality selector
- Favorites/bookmarks
- And more!

---

**Enjoy streaming! 📺✨**
