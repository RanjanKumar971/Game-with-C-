# 🌲 Timber Game with SFML

A fun C++ game built with SFML where you chop down trees while avoiding falling branches. Inspired by the classic *Timberman*.

---

## 🎮 How to Play
- Press `Enter` to start the game
- Press `Left Arrow` or `Right Arrow` to chop on that side
- Avoid falling branches or you lose
- Keep chopping to beat the timer and increase your score
- Press ESC to close the window

---

## 📸 Screenshot

![Gameplay](https://github.com/RanjanKumar971/Game-with-C-/blob/main/graphics/startscreen.png)

---

## 🛠️ Installing MinGW and SFML (Windows)

### 🔧 Step 1: Install MinGW (C++ Compiler)

1. Download MinGW from [MinGW SourceForge](https://sourceforge.net/projects/mingw/).
2. During installation, make sure to select:
   - `mingw32-gcc-g++`
   - `mingw32-base`
3. After installation, add MinGW’s `bin` folder to your system `PATH`:
   - Usually: `C:\MinGW\bin`

4. Verify installation:
   ```bash
   g++ --version
   ```

---

### 🖼️ Step 2: Install SFML

1. Download the **GCC 7.3.0 MinGW (32-bit)** version of SFML from [SFML Downloads](https://www.sfml-dev.org/download.php).
2. Extract the contents to a location of your choice (e.g., `C:\SFML`).

---

### ⚙️ Step 3: Compile the Game

```bash
g++ -IC:/SFML/include -LC:/SFML/lib timber.cpp -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio -o timber.exe
```

> 🔁 Adjust the `C:/SFML` path if you installed it elsewhere.

---

### 🧩 Step 4: Add Required DLLs

Copy the following DLLs from `C:\SFML\bin` to your project directory (next to `timber.exe`):

- `sfml-graphics-2.dll`
- `sfml-window-2.dll`
- `sfml-system-2.dll`
- `sfml-audio-2.dll`

---

### ✅ Run the Game

```bash
./timber.exe
```

Enjoy chopping some trees! 🌲🪓

---

## 📁 Folder Structure

```
.
├── graphics/
│   ├── background.png
│   ├── tree.png
│   ├── cloud.png
│   ├── bee.png
│   ├── player.png
│   ├── axe.png
│   ├── log.png
│   ├── rip.png
│   └── screenshot.png
├── sound/
│   ├── chop.wav
│   ├── death.wav
│   └── out_of_time.wav
├── fonts/
│   └── KOMIKAP_.ttf
├── timber.cpp
├── .gitignore
└── README.md
```

---

## 🧠 Credits
- Developed using [SFML](https://www.sfml-dev.org/)
- Inspired by the classic *Timberman* game
- Beginning C++ Game Programming: Learn to Program with C++ by Building Fun Games by John Horton, 2019


---

Feel free to fork, play around, or contribute 🚀

