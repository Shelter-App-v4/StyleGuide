# Frontend
## Style guide
The style guide concerns colors, fonts, spacing and component design. It should be followed to create the most consistent application possible. 
1. Colors
    * The colors used in the application should be directly imported from [app/config/colors.ts](https://github.com/MathiasAAU/ShelterApp-Frontend/blob/main/app/config/colors.ts "app/config/colors.ts") in order to maintain consistent use of colors. 
    * Colors must never be hardcoded! 
    * Future developers is of course allowed to change colors in `colors.ts` if needed. 

2. Fonts
    * `Roboto` (Android) and `Avenir` (iOS). The fonts used can be found in [app/config/styles.ts](https://github.com/MathiasAAU/ShelterApp-Frontend/blob/main/app/config/styles.ts "app/config/styles.ts"). These should also be directly imported from this file. 
    * Fonts should never be hardcoded! 
    * Future developers is of course allowed to change fonts in `styles.ts` if needed.

3. Spacing
    * All screens should implement the `Screen.tsx`-component ([app/components/Screen.tsx](https://github.com/MathiasAAU/ShelterApp-Frontend/blob/main/app/components/Screen.tsx "app/components/Screen.tsx")) in order to keep all UI-elements in a safe view both on Android and iOS. 
    * Spacing between components can differentiate across screens, however, we recommend between `5` and `20` (either `5`, `10`, `15` or `20`). 

4. Component design
    * All component must be styled with a `border-radius` to round-off the edges.
    * Try to avoid `stack-navigation` when clicking functionality of a screen, instead use `modals` to refrain from complex navigation structures in the app.

## Color palette
The ShelterApp should use two main colors, with 3 different shades, which complement each other:
1. Primary: Green
   * Medium: ![#2E9E83](https://via.placeholder.com/15/2E9E83/000000?text=+) `#2E9E83`
   * Light: ![#88b1a7](https://via.placeholder.com/15/88b1a7/000000?text=+) `#88b1a7`
   * Dark: ![#126450](https://via.placeholder.com/15/126450/000000?text=+) `#126450`
2. Secondary: Orange
   * Medium: ![#FFA24D](https://via.placeholder.com/15/FFA24D/000000?text=+) `#FFA24D`
   * Light: ![#FFCC9D](https://via.placeholder.com/15/FFCC9D/000000?text=+) `#FFCC9D`
   * Dark: ![#FF7A00](https://via.placeholder.com/15/FF7A00/000000?text=+) `#FF7A00`

Furthermore, the application uses background- and text colors in shades of grey and a _danger_ color for alerts and deletion. These colors are: 
1. Background: Light grey
   * Medium: ![#DADADA](https://via.placeholder.com/15/DADADA/000000?text=+) `#DADADA`
   * Light: ![#EBEBEB](https://via.placeholder.com/15/EBEBEB/000000?text=+) `#EBEBEB`
   * Dark: ![#D3D3D3](https://via.placeholder.com/15/D3D3D3/000000?text=+) `#D3D3D3`
3. Text: Dark grey
   * Medium: ![#3D3D3D](https://via.placeholder.com/15/3D3D3D/000000?text=+) `#3D3D3D`
   * Light: ![#9A9A9A](https://via.placeholder.com/15/9A9A9A/000000?text=+) `#9A9A9A`
   * Dark: ![#181818](https://via.placeholder.com/15/181818/000000?text=+) `#181818`
5. Danger: Red
   * ![#ff5252](https://via.placeholder.com/15/ff5252/000000?text=+) `#ff5252`

All colors is located in [app/config/colors.ts](https://github.com/MathiasAAU/ShelterApp-Frontend/blob/main/app/config/colors.ts "app/config/colors.ts") and should be imported from this file. Colors should never be hardcoded.

# How to install IOS/Android simulators
IOS:
https://docs.expo.io/workflow/ios-simulator/  
Android:
https://docs.expo.io/workflow/android-studio-emulator/  
# How to run the app in development
1. `npm install`
2. `npm start` or `expo start`
3. A tab will be opened in your browser with Metro Bundler
4. Open IOS/Android simulator from Metro Bundler or Expo in the terminal
# How to test the app on your personal device  
1. Download Expo Client from your app store  
2. Open camera scan the barcode provided from expo in your terminal or from the Metro Bundler  
3. Expo Client should open the app automatically on your phone

# How to run tests
1. UI tests -> `npm run ui`
2. Integration tests -> `npm run integration`
3. All tests -> `npm test`

# Tips & Tricks
### ts-standard:
This project uses ts-standard(the ts version of standardjs). Using the standardjs plugin for your editor makes it complain in real time as you write your code - this will happen a lot, don't you worry :) It also enables you to auto fix most syntax errors with 'formatOnSave' feature in your editor(same as running ts-standard --fix). REMEMBER: to choose the ts-standard engine in your settings(standardjs is default), so your editor gives you the correct help.
### Debugging: 
I strongly recommend using React Native Debugger from jhen0409. It's 3 react debuggers combined into one tool. 

https://github.com/jhen0409/react-native-debugger
 
