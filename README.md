# Spotify News Studio - With Local Fonts & PIN Protection

## Setup Complete! ✓

Your News Studio is now configured to use local Spotify Mix fonts that will work on any computer and is protected with a PIN.

## 🔒 PIN Protection

**Default PIN: `1234`**

To change the PIN:
1. Open `index.html` in a text editor
2. Find line: `const CORRECT_PIN = '1234';`
3. Change `'1234'` to your desired PIN
4. Save the file

**Security Note:** The PIN is stored in the HTML file. This provides basic protection but is not enterprise-grade security. For more secure authentication, consider server-side solutions.

## File Structure

```
news-studio/
├── index.html          (Your updated HTML file)
├── fonts/
│   ├── SpotifyMixOffcWide-BlackItalic.ttf
│   ├── SpotifyMix-Regular.otf
│   └── SpotifyMix-Light.otf
└── README.md
```

## How to Use

1. **Open the tool**: Simply double-click `index.html` or open it in any browser
2. **Share with others**: Send the entire `news-studio` folder to anyone
3. **Deploy online**: Upload all files to any web server, keeping the folder structure intact

## Important Notes

- ✅ Fonts will now work on ANY computer
- ✅ No internet required for fonts to load
- ✅ Keep the `fonts` folder together with `index.html`
- ✅ All font files must stay in the `fonts/` subfolder

## Deployment

To deploy this to a web server:
1. Upload the entire `news-studio` folder
2. Make sure folder structure stays intact
3. Access via `https://yoursite.com/news-studio/index.html`

## Troubleshooting

If fonts don't load:
- Check that font files are in the `fonts/` folder
- Make sure font file names match exactly:
  - SpotifyMixOffcWide-BlackItalic.ttf
  - SpotifyMix-Regular.otf
  - SpotifyMix-Light.otf
- Open browser console (F12) to check for errors

---

**Created with Claude Code**
