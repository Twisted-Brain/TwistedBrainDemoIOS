# TwistedBrain Demo iOS

A simple OpenFL Haxe demo application for iOS showcasing TwistedBrain graphics.

## Features

- Interactive logo display with click-to-cycle functionality
- Uses TwistedBrain logo assets (tb.png, tb_2.png, tb_3.png, tb_4.png, tb_5.png)
- Clean, simple UI with welcome text and instructions
- Built specifically for iOS target

## Project Structure

```
TwistedBrainDemoIOS/
├── project.xml              # OpenFL project configuration
├── Source/
│   └── TwistedBrainDemoMain.hx  # Main application class
├── Assets/
│   ├── tb.png               # TwistedBrain logo variants
│   ├── tb_2.png
│   ├── tb_3.png
│   ├── tb_4.png
│   └── tb_5.png
└── Export/
    └── ios/
        ├── TwistedBrainDemo.xcodeproj  # Xcode project
        └── build/
            └── Release-iphonesimulator/
                └── TwistedBrainDemo.app  # Built iOS application
```

## Requirements

- Haxe 4.3.7+
- OpenFL 9.4.1+
- Lime 8.2.2+
- iOS development environment (Xcode)
- Apple Developer Account (for device deployment)

## Building

1. Navigate to the project directory:
   ```bash
   cd TwistedBrainDemoIOS
   ```

2. Build for iOS:
   ```bash
   haxelib run openfl build ios
   ```

3. Open in Xcode and run:
   ```bash
   open Export/ios/TwistedBrainDemo.xcodeproj
   ```

4. Select iOS Simulator or connected device and press Play (▶️) in Xcode

## Usage

- The application displays a welcome message and the first TwistedBrain logo
- Click anywhere on the screen to cycle through the different logo variants
- The application window is 800x600 pixels with a black background

## Development Notes

- Main class: `TwistedBrainDemoMain`
- Package: `com.twistedbrain.demo`
- Target FPS: 60
- Hardware acceleration enabled
- VSync enabled for smooth rendering

## Assets

All logo assets are sourced from the TB-graphics collection and are automatically embedded in the application during build.