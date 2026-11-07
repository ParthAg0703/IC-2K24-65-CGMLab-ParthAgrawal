# CGM Lab Assignment 1 – Basic Shapes

Draws four basic shapes in a graphics window using the built-in `graphics.h` functions, each with a text label.

## Files

| File | Description |
|---|---|
| `Basic_shapes.cpp` | Source code |
| `Basic_shapes.exe` | Compiled Windows executable |
| `output.png` | Screenshot of the output |

## What It Draws

| Shape | Function used | Details |
|---|---|---|
| Line | `line()` | Horizontal line from (100, 100) to (300, 100) |
| Circle | `circle()` | Center (200, 250), radius 70 |
| Rectangle | `rectangle()` | Corners (400, 100) and (600, 250) |
| Triangle | three `line()` calls | Vertices (450, 350), (550, 450) and (350, 450) |

Each shape is labelled using `outtextxy()`.

## Run

Run `Basic_shapes.exe` on Windows, or compile `Basic_shapes.cpp` with a compiler that has `graphics.h`. Press any key to close the window (the program waits with `getch()`).

## Concepts

`initgraph()` with `DETECT` for automatic driver selection, screen coordinates (origin at top-left, y increases downward), drawing a polygon from line segments.
