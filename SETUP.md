# Quick Setup Guide

## 🚀 Get Started in 2 Minutes

### Step 1: Download/Clone the Repository
```bash
git clone https://github.com/alexelgato61-design/iptv_complated_work.git
cd iptv_complated_work
```

### Step 2: Start the Server

Choose one method:

**Option A: Python (Easiest)**
```bash
python3 -m http.server 8000
```

**Option B: Node.js**
```bash
npx http-server -p 8000
```

**Option C: PHP**
```bash
php -S localhost:8000
```

### Step 3: Open in Browser
Navigate to: **http://localhost:8000**

That's it! 🎉

## 🎬 How to Use

1. **Select a Channel**: Click any channel from the list on the right
2. **Custom Stream**: Paste any stream URL in the input field and click "Load"
3. **Load Playlist**: Click "Load Playlist" to refresh the channel list

## 📝 Adding Your Own Channels

Edit `playlist.m3u`:
```m3u
#EXTM3U
#EXTINF:-1,My Channel Name
http://your-stream-url.com/stream.m3u8
```

Then reload the page!

## ❓ Common Issues

**Port 8000 already in use?**
- Use a different port: `python3 -m http.server 8080`
- Then visit: `http://localhost:8080`

**Video not playing?**
- Check the stream URL is valid
- Try a different browser
- Check your internet connection

## 🌟 Features

- ✅ No installation needed
- ✅ Works on all platforms
- ✅ Mobile responsive
- ✅ Multiple format support
- ✅ Clean, modern UI

Enjoy streaming! 📺
