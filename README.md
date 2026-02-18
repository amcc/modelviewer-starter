# ModelViewer Demo 🎨

A modern, interactive 3D model viewer built with Google's <em>model-viewer</em> web component. View, interact with, and download 3D models in GLB/GLTF format with support for Augmented Reality.

## 📚 Resources

- **[Model Viewer Official Site](https://modelviewer.dev/)** - Main documentation and examples

## Quick Start

### Option 1: VSCode with Live Server (Recommended)

1. Open the project folder in VSCode
2. Install the **Live Server** extension by Ritwick Dey
   - Open Extensions (Cmd+Shift+X on Mac)
   - Search for "Live Server"
   - Click Install
3. Click "Go Live" in the bottom right of the window, or right-click on `index.html` and select "Open with Live Server"
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

## Adding Your Own GLB Files

### Method 1: Modify HTML

Edit `index.html` and change the `src` attribute in the `<model-viewer>` tag:

```html
<model-viewer src="path/to/your/model.glb" ...> </model-viewer>
```

### Method 2: Reference Remote URLs

Replace the `src` with any publicly accessible GLB URL:

```html
<model-viewer src="https://example.com/path/to/model.glb" ...> </model-viewer>
```

## GLB/GLTF Format Info

- **GLB** - Binary glTF format (recommended, single file)
- **GLTF** - JSON-based format with separate texture files

Both formats are fully supported by Model Viewer.

## Resources

- [Google Model Viewer Docs](https://modelviewer.dev/)
- [Model Viewer GitHub](https://github.com/google/model-viewer)
- [glTF Format Spec](https://www.khronos.org/gltf/)
- [Free 3D Models](https://sketchfab.com/) - Find GLB models to use

## License

This demo uses Google's Model Viewer library, which is licensed under the Apache License 2.0.
