
# 🎮 Pixel Pairs - Memory Match Game  

Pixel Pairs is a memory matching game built using React Native for Android devices. Flip the cards, find the emoji pairs, and beat your best score!

![Game Screenshot](./assets/images/emoji1.png

- Clean, fullscreen game interface (no navigation bar, no status bar)
- 4x5 grid with 10 unique emoji pairs (for fair gameplay)
- Confetti animation and win modal on game completion
- Smooth touch flip animation and sound effects support
- Responsive and modern UI using React Native components
- No third-party ads

***

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/)
- [npm](https://npmjs.com/) or [Yarn](https://yarnpkg.com/)
- [Android Studio](https://developer.android.com/studio) set up for React Native (or use Expo Go for quick testing)
- [ADB](https://developer.android.com/studio/command-line/adb) for APK install

### Installation

Clone this repository:

```bash
git clone https://github.com/yourusername/pixel-pairs.git
cd pixel-pairs
```

Install dependencies:

```bash
npm install
# or
yarn install
```

### Running the App (Development)

**Metro Server:**

```bash
npx react-native start
```

**On Android Device or Emulator:**

```bash
npx react-native run-android
```
> For Expo users:  
> `npx expo start`  
> (then scan the QR code in Expo Go)

***

## 🛠 Building Release APK

1. Make sure your keystore is set up (see [Signing Config Docs](https://reactnative.dev/docs/signed-apk-android)).
2. Run from project root:

```bash
cd android
./gradlew assembleRelease
```
3. Find your APK at:  
   `android/app/build/outputs/apk/release/app-release.apk`

4. **If you get an INSTALL_FAILED_UPDATE_INCOMPATIBLE error:**  
   Uninstall old versions before installing release builds:
```bash
adb uninstall com.pixelpairs
adb install android/app/build/outputs/apk/release/app-release.apk
```

***

## 📦 Folder Structure

```
.
├── App.js
├── assets/
│   └── images/
│       ├── emoji1.png
│       ├── emoji2.png
│       └── ...
├── src/
│   └── Component/
│       └── screen/
│           └── GameScreen.jsx
├── android/
├── ios/
├── package.json
└── README.md
```

***

## 📝 Customization

- Change emoji images by replacing files in `assets/images/`
- For different grid sizes or themes, edit constants at the top of `GameScreen.jsx`
- To change the app name/icon, update `app.json` (Expo) or `android/app/src/main/res/` (vanilla RN)

***

## ✍️ Credits

- Game logic and idea by [Ashwin]
- Built with [React Native](https://reactnative.dev/)
- Emoji art via [your emoji/image source, if applicable]

***

## 📃 License

This project is open-source under the [MIT License](LICENSE).

***

## 🙋 Contributing

Feel free to submit issues, pull requests, or suggestions!  
Star this repo if you enjoy playing Pixel Pairs!

***

**Enjoy playing and improving your memory with Pixel Pairs!**

