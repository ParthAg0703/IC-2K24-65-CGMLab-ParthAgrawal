# Computer Graphics and Multimedia Lab – IC-2K24-65

Lab assignments for the **Computer Graphics and Multimedia (CGM) Lab** course, **5-Year Integrated MCA, IIPS DAVV**.

| | |
|---|---|
| **Student** | Parth Agrawal |
| **Roll No.** | IC-2K24-65 |
| **Institute** | International Institute of Professional Studies (IIPS), DAVV, Indore |
| **Language** | C++ with `graphics.h` (WinBGIm / BGI) |

## Repository Structure

| Folder | Topic | What's inside |
|---|---|---|
| [CGM Lab Assignment1](CGM%20Lab%20Assignment1/) | Basic shapes | Line, circle, rectangle and triangle using built-in graphics functions |
| [CGM Lab Assignment2](CGM%20Lab%20Assignment2/) | DDA line algorithm | Line drawing with the Digital Differential Analyzer algorithm |

Each folder has the source (`.cpp`), a compiled Windows executable (`.exe`) and a screenshot of the output (`output.png`).

## Requirements

- A C++ compiler such as MinGW (g++)
- The `graphics.h` library (WinBGIm), which is not part of standard C++

## How to Compile and Run

With MinGW and WinBGIm installed:

```bash
g++ "CGM Lab Assignment1/Basic_shapes.cpp" -o Basic_shapes -lbgi -lgdi32 -lcomdlg32 -luuid -loleaut32 -lole32
./Basic_shapes
```

The exact linker flags depend on how WinBGIm is set up on your machine. The `.exe` files in the repo run directly on Windows without compiling.

## Concepts Covered

- Initializing the graphics window with `initgraph()` and closing it with `closegraph()`
- Drawing primitives: `line()`, `circle()`, `rectangle()`, `outtextxy()`
- Pixel-level plotting with `putpixel()`
- Incremental line drawing (DDA)
