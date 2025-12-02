
####folder for videos and phtos
https://drive.google.com/drive/folders/17M8c0dqSrHocCGFcP5Uxm4c_E4jFQ8Uh?usp=sharing

## Introduction

This project implements the CometChat UI Kit Builder to integrate real-time chat features into a React application. 
The overall process involved designing the UI inside CometChat’s UI Kit Builder, enabling required features from the 
CometChat Dashboard, exporting the generated code, and integrating it into my existing React project.

### Steps I Followed:
1. **Launched the UI Kit Builder**  
   Logged into the CometChat Dashboard, selected my app, and opened the UI Kit Builder through  
   Integrate → React → Launch UI Kit Builder.

2. **Designed the Chat Interface**  
   Customized layouts, themes, message components, and selected the features I wanted in the chat experience.

3. **Enabled Required Features in Dashboard**  
   Turned on features such as Stickers, Polls, Whiteboard, Document Collaboration, Message Translation, etc.,  
   from Chat → Features.

4. **Exported the UI Kit Code**  
   Downloaded the generated code package which includes components, layouts, contexts, utilities, and theme files.

5. **Integrated the Code into My React App**  
   - Installed required dependencies: `@cometchat/chat-uikit-react` and `@cometchat/calls-sdk-javascript`.  
   - Copied the exported `CometChat` folder into my project’s `src` directory.  
   - Added CometChat credentials (App ID, Region, Auth Key).  
   - Initialized CometChatUIKit inside `main.tsx` and logged in the test user.

6. **Ran and Tested the Application**  
   Started the development server and tested all chat functionalities, themes, popup components, reactions,  
   and feature enablement to ensure everything worked as expected.


## Known Issues & Recommendations

### Dashboard Issues
- UI overlap in Moderation → Get Started page.
- Settings screen opens multiple times and requires multiple back presses.
- Custom graph shows placeholder text instead of actual data.
- UI flickering and delayed rendering on page load.
- Copy button positioned incorrectly above the copy layout area.

### UI Kit Builder Issues
- "New Group" popup UI is cut off in phone mode.
- Emoji picker overflows outside phone preview frame.
- Voice recorder UI does not close on outside click.

### Documentation Issues
- No clear step-by-step integration flow.
- UI Kit Builder sections (Layout, Theme, Features) not explained clearly.
- Missing details about dependency versions and conflicts.
- Preview setup instructions unclear.
- No troubleshooting/known issues section.

### UI Kit Implementation Issues
- Missing "Report User" option in User Info panel.
- Emoji reactions display differently in exported code vs UI Kit Builder preview.
- App layout not rendering fullscreen; background not fitting properly.

### General Recommendation
Improve layout responsiveness, fix popup closing behavior, align exported UI with Builder preview, and enhance documentation with clearer flow and troubleshooting steps.

### Technologies Used
- **React.js** – Base frontend framework for the application  
- **Vite** – Fast development environment and project bundler  
- **TypeScript** – Strongly typed development for reliability  
- **CometChat UI Kit Builder** – Used to design and customize chat UI  
- **CometChat Chat UI Kit (React SDK)** – Integrates chat components into the app  
- **CometChat Calls SDK** – Adds calling/audio/video features  
- **CometChat Dashboard** – Enabled chat features and managed app settings  




# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default defineConfig([
  globalIgnores(["dist"]),
  {
    files: ["**/*.{ts,tsx}"],
    extends: [
      // Other configs...

      // Remove tseslint.configs.recommended and replace with this
      tseslint.configs.recommendedTypeChecked,
      // Alternatively, use this for stricter rules
      tseslint.configs.strictTypeChecked,
      // Optionally, add this for stylistic rules
      tseslint.configs.stylisticTypeChecked,

      // Other configs...
    ],
    languageOptions: {
      parserOptions: {
        project: ["./tsconfig.node.json", "./tsconfig.app.json"],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
]);
```

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from "eslint-plugin-react-x";
import reactDom from "eslint-plugin-react-dom";

export default defineConfig([
  globalIgnores(["dist"]),
  {
    files: ["**/*.{ts,tsx}"],
    extends: [
      // Other configs...
      // Enable lint rules for React
      reactX.configs["recommended-typescript"],
      // Enable lint rules for React DOM
      reactDom.configs.recommended,
    ],
    languageOptions: {
      parserOptions: {
        project: ["./tsconfig.node.json", "./tsconfig.app.json"],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
]);
```

=======

# CometChat

> > > > > > > 24345bc024a55a55b39a235453b460a9c1c664b6
