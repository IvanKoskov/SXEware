# SXEware
[![Platform](https://img.shields.io/badge/Platform-MacOS-blue.svg)](https://developer.apple.com/MacOS/)
[![Platform](https://img.shields.io/badge/Platform-Linux-blue.svg)](https://www.linux.org/)


<p align="center">
    <a href="https://github.com/IvanKoskov/SXEware/blob/main/LICENSE">
        <img src="https://img.shields.io/github/license/IvanKoskov/SXEware?style=for-the-badge">
    </a>
    </br>
    <img src="https://img.shields.io/depfu/dependencies/github/IvanKoskov/SXEware?style=for-the-badge" alt="">
    <img src="https://img.shields.io/github/languages/top/IvanKoskov/SXEware?style=for-the-badge" alt="Language Badge">
    <a href="https://github.com/IvanKoskov/Shellman/actions">
        <img src="https://img.shields.io/github/workflow/status/IvanKoskov/Shellman/CI?style=for-the-badge" alt="Build Status">
    </a>
    <img src="https://img.shields.io/github/issues/IvanKoskov/SXEware?style=for-the-badge" alt="Issues">
    <img src="https://img.shields.io/github/issues-pr/IvanKoskov/SXEware?style=for-the-badge" alt="Pull Requests">
    <img src="https://img.shields.io/github/contributors/IvanKoskov/SXEware?style=for-the-badge" alt="Contributors">
    <img src="https://img.shields.io/github/last-commit/IvanKoskov/SXEware?style=for-the-badge" alt="Last Commit">
</p>



A lightweight tool for listening to music across different platforms.

## Features
- Play music from local files and online sources.
- Save your favorite tracks.
- Load playlists from files.
- Full support for free music and streaming websites.
- Clean and customizable interface using OpenGL (ImGui, C).

## Requirements
- **Operating System:** macOS, Linux, or Windows (manual adjustments required).
- **Compiler:** C++17 or later.
- **Build System:** CMake.

## Installation & Usage
1. **Clone the repository:**  
   ```sh
   git clone https://github.com/your-repo/SXEware.git
   cd SXEware
   ```
2. **Build the project using CMake:**  
   ```sh
   mkdir build && cd build
   cmake ..
   make
   ```
3. **Run the application:**  
   - On **Linux/macOS**: Use the generated executable.
   - On **Windows**: Adjust paths and dependencies manually.

4. **Customize the ImGui interface** to fit your needs.

## Default Music Directory
By default, the application looks for music in:
```
/Users/yourname/Musics/Metamorphosis.wav
```
Modify this path in the settings or source code to change the default music directory.

## Contributing
Feel free to extend and modify this project to suit your needs. Contributions are welcome!

## Licence
GPL

