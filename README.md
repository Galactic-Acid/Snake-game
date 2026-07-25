# 🐍 Classic Snake Game in Java

> An interactive 2D Snake game built from scratch using Java, Swing GUI, and Object-Oriented Programming (OOP) principles.

![Java](https://img.shields.io/badge/Language-Java-orange?style=flat-square&logo=java)
![GUI](https://img.shields.io/badge/Framework-Java%20Swing%20%2F%20AWT-blue?style=flat-square)
![Release](https://img.shields.io/badge/Release-v1.01-brightgreen?style=flat-square)
![Status](https://img.shields.io/badge/Status-Completed-success?style=flat-square)

![snakecopy](https://github.com/user-attachments/assets/d5d5af83-f7d4-4028-9b34-16eb2d5cb0b5)

---

## 🎮 Download & Play

**Latest Version:** `v1.01` (Executable `.jar`)

👉 **[Click Here to Download the Executable JAR from Releases](https://github.com/GaLactic-Acid/Snake-game/tags)**

*(Requires Java Runtime Environment (JRE) installed on your system).*

---

## 🛠️ Technical Stack & Architecture

| Category | Component / Concept |
| :--- | :--- |
| **Language** | Java 8+ |
| **GUI Framework** | Java Swing (`JFrame`, `JPanel`, `JButton`) & AWT (`Graphics`, `Color`) |
| **Event Architecture** | `ActionListener`, `KeyListener`, `MouseListener`, `javax.swing.Timer` |
| **Data Structures** | `ArrayList` (Dynamic coordinate management for snake body rectangles) |

---

## 💡 Key Features Implemented

* **Dynamic Snake Growth:** Eating pellets appends new rectangle segments to the `snakeBody` array list and updates game score dynamically.
* **Smart Input Locking:** Prevents instant reverse movement (e.g., traveling upward and immediately pressing down) to maintain valid state transitions.
* **Custom Graphics & UI:** Custom-rendered grid, directional eyes for the snake head, overlay end screens, and an interactive reset button.
* **Standalone Deployment:** Fully packaged executable `.jar` file with classpath-resolved resource loading for UI assets and icons.

---

## 📅 Development Progress Log

<details>
<summary><b>Click to expand full development timeline & commit history</b></summary>

<br>

*(Refer to the GitHub repository's commit history to track code development in greater detail.)*

*Progress prior to logging can be found in the GitHub commit history.*

### 🗓️ December 2024
* **25/12/2024:**
  * Started logging development progress.
  * Added `checkbounds` (ensuring the snake stays within window boundaries).
  * Successfully utilized `ArrayList` for `Rectangles` (snake body segments) and dynamic coordinate updating.
  * Learned and implemented `ActionListener`, `KeyListener`, and `Timer`.
  * Implemented pellet interactions: snake growth upon eating a pellet (`snakeBody` expansion) and random pellet coordinate generation.
* **26/12/2024:**
  * Added `paintScore` in `MyPanel.java` to display live score and size increases.
  * Added self-collision detection logic.
  * Built `endScreen` showing Game Over state and final score.
  * **Finished core game loop of Snake.**
  * Fixed off-screen window boundary bugs.
  * Cleaned up redundant code inside `actionPerformed` in `MyPanel.java`.
* **28/12/2024:**
  * Resolved illegal direction bug in `MyPanel.java`'s `actionPerformed` method (prevented immediate opposite movement).
  * **Published First Pre-release (`v1.0`) in executable JAR format.**
* **29/12/2024:**
  * Implemented interactive reset button.

---

### 🗓️ January – April 2025
* **05/01/2025:** Fixed endless boundary calculation issues.
* **24/03/2025:** Rendered directional eyes onto the snake's head segment.
* **11/04/2025:** **Released Version 1.01 (Executable JAR)**.
* **12/04/2025:**
  * Fixed eye directional bug caused by unaccounted user input states.
  * Fixed `v1.01` JAR launch error (`A Java exception has occurred`) by moving reset icons and images into the `src` folder for proper classpath bundling.
  * Restored visibility for the reset button icon.
  * Dropped native `.exe` build support in favor of pure cross-platform Java `.jar`.

</details>

---

## 🔮 Future Roadmap & Improvements

- [ ] **AI Game Mode:** Implement computer-driven pathfinding/autonomous play.
- [ ] **Dynamic Obstacles:** Introduce obstacles and progressive difficulty scaling over time.
- [ ] **Main Menu UI:** Add a start menu to select difficulty and game modes.
- [ ] **Enhanced Visuals:** Animate snake movement (tongue interval animations, smoother transition frames).
- [ ] **Code Refactoring:** Refine `Snake.java` eye rendering logic for better readability and maintainability.
- [ ] **Customization:** Add options for custom snake colors and adjustable game speed.

---

## 📚 References & Learning Resources

All resources and tutorials utilized during the development of this project:
* **2D Graphics in Java:** [YouTube Video: Java 2D canvas graphics](https://www.youtube.com/watch?v=KcEvHq8Pqs0&t=426ss)
* **Java MouseListener Integration:** [YouTube Video:Java MouseListener](https://www.youtube.com/watch?v=jptf1Wd_omw)
* **GUI Reset Button Implementation:** [YouTube Video: Java - reset button for your game](https://www.youtube.com/watch?v=cA1GvZ5Y3-U)
* **Invisible/Clickable JButton Tricks:** [Stack Overflow Discussion](https://stackoverflow.com/questions/5654208/making-a-jbutton-invisible-but-clickable)

---
*Created by Hrithik Singh*
