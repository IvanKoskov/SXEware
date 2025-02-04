# SXEware
[![Platform](https://img.shields.io/badge/Platform-MacOS-blue.svg)](https://developer.apple.com/MacOS/)
[![Platform](https://img.shields.io/badge/Platform-Linux-blue.svg)](https://www.linux.org/)


<p align="center">
    <a href="https://github.com/IvanKoskov/SXEware/blob/main/LICENSE">
        <img src="https://img.shields.io/github/license/IvanKoskov/SXEware?style=for-the-badge">
    </a>
    </br>
    <img src="https://img.shields.io/github/languages/top/IvanKoskov/SXEware?style=for-the-badge" alt="Language Badge">
    <a href="https://github.com/IvanKoskov/Shellman/actions">
        <img src="https://img.shields.io/github/workflow/status/IvanKoskov/Shellman/CI?style=for-the-badge" alt="Build Status">
    </a>
    <img src="https://img.shields.io/github/issues/IvanKoskov/SXEware?style=for-the-badge" alt="Issues">
    <img src="https://img.shields.io/github/issues-pr/IvanKoskov/SXEware?style=for-the-badge" alt="Pull Requests">
    <img src="https://img.shields.io/github/contributors/IvanKoskov/SXEware?style=for-the-badge" alt="Contributors">
    <img src="https://img.shields.io/github/last-commit/IvanKoskov/SXEware?style=for-the-badge" alt="Last Commit">
</p>


<img width="793" alt="Image" src="https://github.com/user-attachments/assets/be38f692-ef41-420b-b985-94448f5f10a8" />



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
> [!IMPORTANT]
> You need to fully setup IMGUI on your machine from the official repository before proceeding with custom builds or etc.

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

# Dependencies for the Music Player

This document lists all the dependencies required for the music player project, including libraries and frameworks used for graphics, audio, and UI.

## Required Dependencies

### 1. **GLFW** (Window and Input Handling)
   - **Purpose:** Creates the OpenGL window and handles user input.
   - **Installation:**
     ```sh
     brew install glfw  # macOS (Homebrew)
     sudo apt install libglfw3-dev  # Linux (APT)
     vcpkg install glfw3  # Windows (vcpkg)
     ```

### 2. **GLAD** (OpenGL Loader)
   - **Purpose:** Loads OpenGL function pointers for compatibility across platforms.
   - **Installation:**
     - Generate the loader at [glad.dav1d.de](https://glad.dav1d.de/)
     - Copy the generated files into your project.

### 3. **OpenAL-Soft** (Audio Playback)
   - **Purpose:** Handles audio playback for `.wav` files.
   - **Installation:**
     ```sh
     brew install openal-soft  # macOS (Homebrew)
     sudo apt install libopenal-dev  # Linux (APT)
     vcpkg install openal-soft  # Windows (vcpkg)
     ```

### 4. **ImGui** (GUI Framework)
   - **Purpose:** Provides the graphical user interface.
   - **Installation:**
     - Clone the repository:
       ```sh
       git clone https://github.com/ocornut/imgui.git
       ```
     - Include necessary files in your project.

### 5. **ImGui Backends** (GLFW and OpenGL Integration)
   - **Purpose:** Connects ImGui with OpenGL and GLFW.
   - **Files to include:**
     - `imgui/backends/imgui_impl_glfw.cpp`
     - `imgui/backends/imgui_impl_glfw.h`
     - `imgui/backends/imgui_impl_opengl3.cpp`
     - `imgui/backends/imgui_impl_opengl3.h`

### 6. **C++ Standard Library**
   - **Purpose:** Handles threading (`std::thread`), atomic operations (`std::atomic`), and file I/O.
   - **Installation:** Included with any modern C++ compiler.

## Optional Dependencies

### 7. **STB Image (For Album Art & Icons)**
   - **Purpose:** Loads image files for future features like album art.
   - **Installation:**
     - Download and place `stb_image.h` from [https://github.com/nothings/stb](https://github.com/nothings/stb) in your project.

### 8. **libmpg123 (MP3 Support - Future Feature)**
   - **Purpose:** Decodes MP3 files if support is added.
   - **Installation:**
     ```sh
     brew install mpg123  # macOS
     sudo apt install libmpg123-dev  # Linux
     vcpkg install mpg123  # Windows
     ```

### 9. **Different headers and etc**
   - **Purpose:** Additional sound support

## Build Instructions
Make sure all dependencies are installed and then build using CMake:

```sh
mkdir build && cd build
cmake ..
make -j$(nproc)  # Linux/macOS
cmake --build .   # Windows (MSVC)
```

---

This list covers all libraries used. Let me know if you need additional dependencies or installation details!





