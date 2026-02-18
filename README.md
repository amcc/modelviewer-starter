# ModelViewer Demo 🎨

A modern, interactive 3D model viewer built with Google's Model Viewer web component. View, interact with, and download 3D models in GLB/GLTF format with support for Augmented Reality.

## 📚 Resources

- **[Model Viewer Official Site](https://modelviewer.dev/)** - Main documentation and examples
- **[Model Viewer API Reference](https://modelviewer.dev/docs/intro)** - Complete API documentation
- **[Model Viewer GitHub](https://github.com/google/model-viewer)** - Source code and issues
- **[glTF Format Spec](https://www.khronos.org/gltf/)** - 3D model format specification

## Features

- 🔄 **Auto-rotate** - Automatically spin the model
- 🎮 **Camera controls** - Click and drag to rotate, scroll to zoom
- 📱 **AR Support** - View models in your real environment (on supported devices)
- 📁 **Custom uploads** - Load your own GLB/GLTF files
- ⬇️ **Download** - Save GLB files to your device
- 📱 **Responsive** - Works great on desktop, tablet, and mobile
- 🎨 **Beautiful UI** - Modern, gradient background with smooth interactions

## Quick Start

### Option 1: VSCode with Live Server (Recommended)

1. Open the project folder in VSCode
2. Install the **Live Server** extension by Ritwick Dey
   - Open Extensions (Cmd+Shift+X on Mac)
   - Search for "Live Server"
   - Click Install
3. Right-click on `index.html` and select "Open with Live Server"
4. Your browser will automatically open and reload on file changes

### Option 2: Use a Local Server

For better compatibility and to test local GLB files:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server)
npx http-server

# Using Node.js (with serve)
npx serve
```

Then navigate to `http://localhost:8000` in your browser.

### Option 3: Open Directly

Simply open `index.html` directly in your web browser. The demo loads the model from your assets folder.

## How to Use

1. **Rotate Model** - Click and drag with your mouse
2. **Zoom** - Use your mouse wheel or pinch on touch devices
3. **Auto-rotate** - Click the "Toggle Auto-Rotate" button
4. **AR Mode** - Click "Toggle AR" button (requires supported device)
5. **Upload Custom Model** - Click the file upload area to load your own GLB/GLTF files
6. **Download** - Click "Download GLB" to save the current model

## Adding Your Own GLB Files

### Method 1: Upload via UI

Click the file upload area and select your GLB/GLTF file.

### Method 2: Modify HTML

Edit `index.html` and change the `src` attribute in the `<model-viewer>` tag:

```html
<model-viewer src="path/to/your/model.glb" ...> </model-viewer>
```

### Method 3: Reference Remote URLs

Replace the `src` with any publicly accessible GLB URL:

```html
<model-viewer src="https://example.com/path/to/model.glb" ...> </model-viewer>
```

## GLB/GLTF Format Info

- **GLB** - Binary glTF format (recommended, single file)
- **GLTF** - JSON-based format with separate texture files

Both formats are fully supported by Model Viewer.

## Browser Support

- ✅ Chrome 83+
- ✅ Firefox 77+
- ✅ Safari 12.1+
- ✅ Edge 83+
- ✅ Mobile browsers with WebGL support

## AR Support

AR viewing requires:

- Device with AR capabilities (most modern smartphones)
- Chrome, Firefox, or Safari mobile browser
- HTTPS connection (or localhost)

## Customization

Edit `index.html` to customize:

- **Colors** - Change the gradient in CSS
- **Model size** - Modify the `height` property in `model-viewer` CSS
- **Camera position** - Adjust `camera-controls` settings
- **Background** - Change `environment-image` attribute
- **Lighting** - Add `lighting` configurations

## Resources

- [Google Model Viewer Docs](https://modelviewer.dev/)
- [Model Viewer GitHub](https://github.com/google/model-viewer)
- [glTF Format Spec](https://www.khronos.org/gltf/)
- [Free 3D Models](https://sketchfab.com/) - Find GLB models to use

## License

This demo uses Google's Model Viewer library, which is licensed under the Apache License 2.0.
