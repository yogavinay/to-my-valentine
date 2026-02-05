# Background Music Setup

## How to Add Your Song

1. **Place your music file here**: Add your `.mp3` or `.ogg` file to this `public/audio/` folder.

2. **Update the path in code**: Open `src/components/HeartPortal.tsx` and update line 18:
   ```typescript
   src: '/audio/your-song.mp3', // Change 'your-song.mp3' to your actual filename
   ```

3. **File recommendations**:
   - **Format**: Use `.mp3` or `.ogg` for best browser compatibility
   - **Size**: Keep under 5MB for fast loading
   - **Loop**: Choose a song that loops smoothly (ends and starts seamlessly)

## How It Works

- The music starts when the user clicks the heart button on the greeting screen
- It fades in smoothly over 8 seconds (from silent to full volume)
- The song loops continuously until the tab is closed
- If the browser blocks audio, check the browser console for error messages

## Troubleshooting

If the music doesn't play:
1. Check the browser console (F12) for error messages
2. Make sure the file path in `HeartPortal.tsx` matches your filename exactly
3. Ensure the file is in the `public/audio/` folder
4. Try a different audio format (.mp3 or .ogg)

