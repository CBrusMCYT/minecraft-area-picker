# 🗺️ Minecraft Area Picker

A lightweight web application for selecting and exporting specific regions from your Minecraft worlds (Java & Bedrock editions).

## Features

✨ **Supported Formats:**
- **Java Edition:** Upload `.zip` world files → Export to `.schem`, `.schematic`, or `.litematic`
- **Bedrock Edition:** Upload `.mcworld` files → Export to `.mcstructure`

🎮 **2D Bird's Eye View:**
- Interactive map rendering showing block types and heights
- Color-coded blocks for easy identification
- Grid overlay for precise positioning

📝 **Height Selection:**
- Y-axis range slider (supports heights from -64 to 320)
- Real-time height display similar to Xaero's Minimap
- Height-based brightness visualization

🎯 **Easy Selection:**
- Click twice on the map to select start and end corners
- Real-time selection information display
- Region size calculation

## Usage

1. **Open the App**
   - Visit the raw HTML file or serve it locally
   - No external dependencies needed

2. **Select World Type**
   - Choose between Java Edition or Bedrock Edition

3. **Upload World**
   - Select your world file (.zip for Java, .mcworld for Bedrock)
   - Maximum file size: 500MB

4. **Select Region**
   - Click on the 2D map to select two corners of your desired region
   - Use the height sliders to define Y-axis range

5. **Export**
   - Choose your preferred export format
   - Click "Export Area" to download

## Technical Details

**Single File Application:**
- Pure HTML/CSS/JavaScript - no build process needed
- No external API calls or dependencies
- Works entirely in the browser
- File size limit: 500MB (browser limitation)

**Supported Block Colors:**
- 🟫 Stone/Cave areas
- 🟫 Dirt
- 🟩 Grass
- 🔵 Water
- 🟨 Sand
- ⚫ Void/Very Low areas

**Height System:**
- Minimum: -64 (Bedrock Edition lowest level)
- Maximum: 320 (Minecraft 1.18+ highest point)
- Real-time brightness adjustment based on height

## Features

### Map Rendering
- 1 pixel = 1 block ratio
- Brightness gradient based on height (Y-axis)
- Grid overlay (16×16 block chunks)
- Selection rectangle overlay

### Selection Tools
- Click-based corner selection
- Real-time coordinate display
- Region size calculator
- Reset selection button

### Export Options
- **Schematic (.schem)** - Modern format
- **Schematic (.schematic)** - Legacy format
- **Litematic (.litematic)** - Litematica mod format
- **MC Structure (.mcstructure)** - Bedrock structures

## Browser Compatibility

✅ Chrome/Edge 60+
✅ Firefox 55+
✅ Safari 12+
✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Limitations

- Maximum file size: 500MB (browser memory limit)
- Processing happens client-side (may take time for large files)
- Block entity data not fully supported in current version

## Future Improvements

- [ ] Full NBT parsing for accurate block rendering
- [ ] LevelDB support for native Bedrock files
- [ ] Entity preservation in exports
- [ ] Biome color mapping
- [ ] Advanced filtering (select by block type)
- [ ] Undo/Redo functionality
- [ ] Custom height maps

## How to Use

### On GitHub (Browser)
1. Go to https://github.com/CBrusMCYT/minecraft-area-picker
2. Click on `index.html`
3. Click the "Raw" button
4. Bookmark or save the page
5. Use directly in your browser

### Locally
```bash
# Clone the repository
git clone https://github.com/CBrusMCYT/minecraft-area-picker.git

# Navigate to folder
cd minecraft-area-picker

# Open in browser
open index.html
# Or on Windows
start index.html
# Or on Linux
xdg-open index.html
```

### With Live Server
```bash
# If you have Node.js and npm
npm install -g http-server

# Run in the project directory
http-server

# Then visit http://localhost:8080
```

## License

MIT License - feel free to use and modify!

## Credits

Inspired by Xaero's Minimap and Chunker world converter.

---

**Made for Minecraft Java & Bedrock Edition**