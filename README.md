# SXEware
[![C++](https://img.shields.io/badge/C-orange.svg)](https://en.wikipedia.org/wiki/C%2B%2B)
[![Platform](https://img.shields.io/badge/Platform-MacOS-blue.svg)](https://developer.apple.com/MacOS/)
[![Platform](https://img.shields.io/badge/Platform-Linux-blue.svg)](https://www.linux.org/)
[![License](https://img.shields.io/badge/License-GPL-green.svg)](https://opensource.org/licenses/GPL)
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

