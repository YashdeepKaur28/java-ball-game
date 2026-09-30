# Ball Game — Multi-threaded Java Swing Game 🎮

A desktop GUI game built with **Java Swing** that demonstrates **multithreading, custom painting, and real-time event handling**. Two balls move across the screen while nine worker threads compete to change their color — the user clicks the matching color button to "win".

## 📸 Preview

<img width="1592" height="1020" alt="image" src="https://github.com/user-attachments/assets/104d3b38-72fb-4d03-bbf7-aec6e314c81a" />


## 📖 Overview

**Ball Game** (originally titled *Game Centered Output*) is a Java Swing application that uses **nine concurrent threads** to continuously repaint two moving balls in random colors. The user tries to match the ball's current color by clicking the corresponding color button on the control panel.

The project was built to practice:
- Java **Swing** components (`JPanel`, `JButton`, `JFrame`, `JLabel`)
- **Custom painting** via `paintComponent(Graphics)`
- **Multithreading** — nine `Thread` subclasses running simultaneously
- **Event handling** via `ActionListener`
- **Layout management** with `BorderLayout` and `null` (absolute positioning)

## ✨ Features

- 🎯 **Two animated balls** moving diagonally across the screen
- 🎨 **Nine color threads** racing to change the ball color
- 🖱️ **10 buttons** — START, STOP, and 8 color selectors
- 🏆 **Win detection** — displays "Win" when the player's chosen color matches the ball
- 🧵 **Live multithreading** — each color runs in its own thread
- 🖼️ **Custom painting** with `Graphics.fillOval()`
- 🚦 **Start / Stop** control for the animation loop


## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | Java (JDK 8+) |
| GUI | Swing (`JFrame`, `JPanel`, `JButton`, `JLabel`) |
| Graphics | `Graphics`, `paintComponent`, `fillOval` |
| Concurrency | `Thread`, `Runnable`, `Thread.sleep` |
| Events | `ActionListener`, `ActionEvent` |
| Layout | `BorderLayout`, absolute positioning |



## 🎮 How to Play

1. Click **START** — the two balls begin moving and the color threads activate.
2. Watch the balls change color rapidly as nine threads compete.
3. Click the color button that **matches the current ball color**.
4. If you match it, **"Win"** appears on screen.
5. Click **STOP** to pause the animation.


## 🧠 Key Concepts Demonstrated

- **Multithreading:** 9 concurrent `Thread` subclasses (`Thread1` through `Thread9`), each competing to repaint the ball in its assigned color
- **Custom rendering:** Overriding `paintComponent(Graphics g)` to draw the balls with `fillOval()` and render win text
- **Thread-safe UI updates:** Using `repaint()` from worker threads (Swing-safe) to trigger repaints on the EDT
- **Event-driven programming:** A single `ActionListener` handling 10 different buttons using `e.getSource()`
- **Color comparison:** Converting colors to RGB integers (`Color.getRGB()`) to test for a match


## 🚀 Future Enhancements

- [ ] Migrate from absolute positioning to proper layout managers
- [ ] Replace `Thread` subclasses with `Runnable` tasks (cleaner)
- [ ] Add difficulty levels (faster/slower thread intervals)
- [ ] Add score tracking and a timer
- [ ] Add sound effects on win
- [ ] Introduce a proper game loop instead of 9 racing threads
- [ ] Add pause/resume instead of stop-only


## 👩‍💻 Author

**Yashdeep Kaur**
- 🎓 B.Tech CSE, Punjabi University, Patiala (2026)
- 💼 Java Full Stack Trainee @ CodeSquadz
- 📧 Email: ykdeep2453@gmail.com
- 🔗 LinkedIn: [yashdeep-kaur-16aa083b1](https://linkedin.com/in/yashdeep-kaur-16aa083b1)
- 🐙 GitHub: [@YashdeepKaur28](https://github.com/YashdeepKaur28)


⭐ If you found this project fun, consider giving it a star!
