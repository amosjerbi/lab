# Color Selector

A comprehensive color picker application available in both web and iOS implementations, designed to provide professional-grade color selection tools similar to Adobe Photoshop's color picker.

## 🌟 Features

### Web Version
- **Advanced Color Picker**: Interactive color selection with square and bar selectors
- **Multiple Color Spaces**: Support for RGB, HSB, Lab, and CMYK color models
- **HTML/CSS Color Matching**: Find the closest HTML/CSS named color to any selected color
- **Web-Safe Colors**: Filter to show only web-safe color palette (216 colors)
- **HTML Color Library**: Access to all 138 standard HTML color names
- **Real-time Color Conversion**: Instant conversion between all supported color formats
- **WebGL Rendering**: High-performance color gradients using WebGL technology

### iOS Version
- **Native SwiftUI Interface**: Modern, responsive iOS design
- **Color History**: Track and revisit previously selected colors (up to 50 colors)
- **Color Information Display**: View detailed color information including:
  - Color name detection
  - Hex values
  - RGB values
  - HSL values
- **Color Converter**: Convert between different color formats
- **Tabbed Interface**: Organized into Color Picker, History, and Converter sections

## 🚀 Getting Started

### Web Version

1. **Live Demo**: Try the web version at [https://ppyne.github.io/colorselector/](https://ppyne.github.io/colorselector/)

2. **Local Setup**:
   ```bash
   cd colorselector-main
   # Open index.html in your browser (Chrome recommended)
   ```

3. **Requirements**:
   - Modern web browser with WebGL support
   - Chrome recommended for best compatibility
   - Tested primarily on macOS

### iOS Version

1. **Prerequisites**:
   - Xcode 12.0 or later
   - iOS 14.0 or later
   - macOS for development

2. **Installation**:
   ```bash
   # Choose one of the iOS implementations
   cd ColorSelector/ColorSelector
   # or
   cd ColorSelectorFresh
   
   # Open the .xcodeproj file in Xcode
   open ColorSelector.xcodeproj
   ```

3. **Build and Run**:
   - Select your target device or simulator
   - Press Cmd+R to build and run

## 📱 Project Structure

```
colorselector-main/
├── colorselector-main/          # Web implementation
│   ├── index.html              # Main web application
│   ├── scripts/                # JavaScript logic
│   │   ├── color.js           # Color conversion utilities
│   │   └── colorselector.js   # Main color selector logic
│   ├── styles/                # CSS and fonts
│   └── images/                # UI assets
├── ColorSelector/             # Primary iOS implementation
│   └── ColorSelector/
│       ├── ColorSelectorApp.swift
│       ├── ContentView.swift
│       ├── ColorModel.swift
│       ├── ColorPickerView.swift
│       ├── ColorHistoryView.swift
│       └── ColorConverterView.swift
├── ColorSelectorFresh/        # Alternative iOS implementation
└── ColorSelectorIOS/          # Standalone iOS files
```

## 🎨 Usage

### Web Interface

1. **Color Selection**:
   - Click and drag in the main color square to select hue and saturation
   - Use the vertical bar to adjust brightness/lightness
   - Switch between color channels (R, G, B, H, S, B, L, a, b)

2. **Color Modes**:
   - **All Colors**: Full color spectrum
   - **Web Colors**: 216 web-safe colors only
   - **HTML Colors**: 138 standard HTML named colors only

3. **Color Information**:
   - View RGB, HSB, Lab, and CMYK values
   - Get hex color codes
   - Find closest HTML color name

### iOS Interface

1. **Color Picker Tab**:
   - Use the native iOS color picker
   - View real-time color information
   - Add colors to history

2. **History Tab**:
   - Browse previously selected colors
   - Tap to reselect a color
   - Automatic timestamp tracking

3. **Converter Tab**:
   - Convert between color formats
   - Input colors in various formats
   - Export color values

## 🛠 Technical Details

### Web Technologies
- **JavaScript ES6+**: Core application logic
- **WebGL**: High-performance color rendering
- **HTML5 Canvas**: Interactive color selection
- **CSS3**: Modern styling and layouts
- **jQuery**: DOM manipulation and event handling

### iOS Technologies
- **SwiftUI**: Modern declarative UI framework
- **ObservableObject**: Reactive data management
- **Color Extensions**: Advanced color manipulation
- **Core Graphics**: Color space conversions

### Color Space Support
- **RGB**: Red, Green, Blue (0-255)
- **HSB/HSV**: Hue, Saturation, Brightness (H: 0-360°, S&B: 0-100%)
- **Lab**: Lightness, a*, b* (CIE Lab color space)
- **CMYK**: Cyan, Magenta, Yellow, Key/Black (0-100%)
- **Hex**: Hexadecimal color codes (#RRGGBB)

## 📸 Screenshots

The web version includes several color space profiles:

- HSB Profile (H) with web colors
- HSB Profile (S) with HTML/CSS colors  
- Lab Profile (a) with HTML/CSS colors
- Multiple color selection modes

*See the `readme_images/` directory for detailed screenshots*

## 🔧 Development

### Web Development
- Modify `scripts/colorselector.js` for core functionality
- Update `scripts/color.js` for color conversion algorithms
- Customize styles in `styles/` directory

### iOS Development
- Core logic in `ColorModel.swift`
- UI components in individual view files
- Follow SwiftUI best practices for reactive updates

## 📋 Requirements

### Web Version
- Modern browser with WebGL support
- JavaScript enabled
- Canvas support

### iOS Version
- iOS 14.0+
- Xcode 12.0+
- Swift 5.0+

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly on target platforms
5. Submit a pull request

## 📄 License

This project is available under the terms specified in the LICENSE file.

## 🐛 Known Issues

- Web version primarily tested on Chrome/macOS
- Some browsers may have WebGL compatibility issues
- iOS versions may have slight differences in color accuracy

## 🚀 Future Enhancements

- [ ] Additional color spaces (XYZ, Luv)
- [ ] Color palette generation
- [ ] Export functionality for color swatches
- [ ] Accessibility improvements
- [ ] Cross-platform color sync
- [ ] Advanced color harmony tools

---

**Note**: This project was originally developed in 2018 and includes both legacy web implementation and modern iOS Swift versions. The web demo remains available for testing and demonstration purposes.
