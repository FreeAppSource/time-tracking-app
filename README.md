# Time Tracking App

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Ajinkya Prabhavale** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `time-tracking-app-ajinkya-prabhavale.sketch` by **Ajinkya Prabhavale**: one route per artboard, with the artboard's layout, colours, images and text.

![Time Tracking App screens](./showcase.jpg)

## 📱 Screens (6 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **01 Splash** · start screen | `src/app/s-01-splash.jsx` | 375 × 812 | 1 |
| 2 | **02 Login** | `src/app/s-02-login.jsx` | 375 × 812 | 2 |
| 3 | **03 Landing  page** | `src/app/s-03-landing-page.jsx` | 375 × 812 | 2 |
| 4 | **04 Create task** | `src/app/s-04-create-task.jsx` | 375 × 812 | 2 |
| 5 | **05 Calendar View** | `src/app/s-05-calendar-view.jsx` | 375 × 812 | 2 |
| 6 | **06 Summary Report** | `src/app/s-06-summary-report.jsx` | 375 × 812 | 2 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Inter, Nunito), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/time-tracking-app> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **iOS Time Tracking App** design by **Ajinkya Prabhavale**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Ajinkya Prabhavale](https://www.sketchappsources.com/contributor/ajinkyaprabhavale) |
| Original design | [iOS Time Tracking App](https://dribbble.com/shots/6900005-Time-Tracking-App) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4083-time-tracking-app-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/King_Ajinkya55> |
| Original file | `time-tracking-app-ajinkya-prabhavale.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "iOS Time Tracking App" by Ajinkya Prabhavale (https://dribbble.com/shots/6900005-Time-Tracking-App), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4083-time-tracking-app-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
