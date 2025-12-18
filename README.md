
# Image Morphing App

A web-based application that creates smooth morphing animations between two images by gradually transforming each pixel from the starting image to the ending image.

## 🌟 Features

- **Upload Two Images**: Select starting and ending square images
- **Pixel-by-Pixel Morphing**: Each pixel gradually transforms from start to end
- **Automatic Normalization**: Images are automatically resized to the same square dimensions
- **Customizable Settings**: Adjust duration, resolution, and output filename
- **Video Export**: Generate MP4 or WebM video files
- **No External Dependencies**: Built with pure HTML5 Canvas and JavaScript
- **Cross-Browser Support**: Works in Chrome, Firefox, and Edge
- **Drag & Drop**: Easy image upload with drag-and-drop support
- **Real-time Preview**: See your uploaded images before generating

## 🚀 Live Demo

You can access the live version of this app at:  
[Your GitHub Pages URL here]

## 🛠️ How to Use

### 1. Upload Images
- Click on "Starting Image" box to upload your first image
- Click on "Ending Image" box to upload your second image
- Alternatively, drag and drop image files onto the boxes
- Supported formats: JPG, PNG, GIF

### 2. Adjust Settings
- **Duration**: Set how long the morphing animation should last (1-10 seconds)
- **Output Name**: Choose the filename for your video (default: morph.mp4)
- **Resolution**: Select square resolution (256×256, 512×512, or 1024×1024 pixels)

### 3. Generate Video
- Click "Generate Morph Video" to create the animation
- Watch the progress bar as the video is created
- Play the resulting video directly in the browser
- Download the video to your computer

## 🔧 Technical Details

### How It Works
1. **Image Normalization**: Both images are resized to the selected square resolution
2. **Pixel Analysis**: The app analyzes RGB values of each pixel in both images
3. **Morphing Algorithm**: Each pixel's color values are interpolated between start and end states
4. **Frame Generation**: Individual frames are created for each step of the animation
5. **Video Encoding**: Frames are combined into a video file using the MediaRecorder API

### Technologies Used
- **HTML5 Canvas**: For image processing and frame rendering
- **MediaRecorder API**: For video encoding and export
- **File API**: For image upload and processing
- **Drag & Drop API**: For user-friendly file uploads
- **Vanilla JavaScript**: No external libraries required

## 📁 Project Structure

```
image-morphing-app/
├── index.html          # Main application file
├── README.md           # This documentation
├── LICENSE             # MIT License file
└── assets/             # (Optional) Additional assets
    ├── screenshots/
    └── examples/
```

## 🌐 Deployment

### Deploy to GitHub Pages
1. Create a new GitHub repository
2. Upload all files to the repository
3. Go to Repository Settings → Pages
4. Select "Deploy from a branch" and choose "main" branch
5. Your app will be available at: `https://[username].github.io/[repository-name]`

### Local Development
1. Clone the repository or download the files
2. Open `index.html` directly in your browser
3. For better development experience, use a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js with http-server
   npx http-server
   ```

## 🖥️ Browser Compatibility

| Browser | Video Recording | Image Processing |
|---------|----------------|------------------|
| Chrome  | ✅ Full support | ✅ Full support |
| Firefox | ✅ Full support | ✅ Full support |
| Edge    | ✅ Full support | ✅ Full support |
| Safari  | ⚠️ Limited | ✅ Full support |

**Note**: Video recording works best in Chrome and Firefox. Safari has limited MediaRecorder support.

## ⚡ Performance Tips

- **Smaller Resolutions**: Use 256×256 or 512×512 for faster processing
- **Shorter Durations**: 3-5 seconds is usually sufficient
- **Similar Images**: Images with similar compositions work best
- **Close Browser Tabs**: Free up memory by closing unnecessary tabs

## 🔍 Troubleshooting

### Common Issues

1. **Upload not working**
   - Check browser console for errors (F12 → Console)
   - Ensure you're uploading image files (JPG, PNG, GIF)
   - Try a different browser

2. **Video generation hangs**
   - Refresh the page and try again
   - Reduce the resolution or duration
   - Use Chrome or Firefox for best results

3. **Video won't play/download**
   - Check if the video finished generating
   - Try a different browser
   - Clear browser cache and retry

4. **Poor quality morphing**
   - Use images with similar compositions
   - Try higher resolution settings
   - Ensure both images are square or similar aspect ratios

### Browser Console Errors

If you encounter issues, check the browser console (F12) for specific error messages. Common errors include:

- **MediaRecorder errors**: Browser doesn't support the selected codec
- **Memory errors**: Images are too large, try smaller resolution
- **CORS errors**: Opening the file locally, use a local server instead

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

### Areas for Improvement
- Add support for more image formats
- Implement advanced morphing algorithms
- Add more customization options
- Improve mobile responsiveness
- Add audio support to videos

## 🙏 Acknowledgments

- Built with pure HTML5, CSS, and JavaScript
- Inspired by traditional image morphing techniques
- Uses modern browser APIs for video creation

## 📧 Contact

For questions, suggestions, or issues, please:
1. Check the troubleshooting section above
2. Open an issue on GitHub
3. Contact the maintainer directly

---

**Enjoy creating amazing morphing animations!** 🎥✨
