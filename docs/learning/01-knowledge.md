# 01 Knowledge Tauri

Date: 09/06/2026 : Author: Mariano Simonin

1.- In the folder src/ -> Live the ui of Hermes
1.1- Buttons, Design, Forms, Screens.
1.2- All in the folder src/ -> Use React + TypeScript

2.- In the folder src-tauri/ -> Live the naitive app
2.1- System permission, filesystem, SQLite, audio and video. -> Things in rust

3.- Inside the folder scr-tauri/ exist two files **Cargo.toml and tauri.conf.json**
******3.1- Cargo.toml -> Define things like version, plugins and compile configurations.
3.2- tauri.conf.json -> Define things like app name, window size, icons, security and permissio

## src-tauri/

1.- main.rs -> This file is the entry point of the desktop binary

Flow: macOS execute hermes-desktop -> get in main() -> main() calls to hermes_desktop_lib:run() -> Tauri runs the app

2.- lib.rs -> Tauri make the app in this file

Flow: Create a Tauri app -> Register Plugins -> Register Comands in Rust for React -> Load configuration the tauri.conf.json -> Execute app

Tauri command, is a function in rust which the frontend can call using TypeScript.

## src/

1.- main.tsx -> It is usually left as a startup file

Flow: Search an HTML element with an id="root" -> Mount React -> Render the app component

2.- App.tsx -> Screen for the demo , invoke serve like a bridge between TS to Rust

For the last

Src/ -> UI/UX
Src-tauri/ -> native capacities

