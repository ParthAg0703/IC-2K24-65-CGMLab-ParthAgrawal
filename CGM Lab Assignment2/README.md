# CGM Lab Assignment 2 – DDA Line Drawing Algorithm

Draws a line between two user-entered points using the **Digital Differential Analyzer (DDA)** algorithm.

## Files

| File | Description |
|---|---|
| `dda.cpp` | Source code |
| `dda.exe` | Compiled Windows executable |
| `output.png` | Screenshot of the output |

## Algorithm

1. Read the endpoints (x1, y1) and (x2, y2)
2. Compute `dx = x2 - x1` and `dy = y2 - y1`
3. `steps = max(|dx|, |dy|)`
4. Compute the increments `xInc = dx / steps` and `yInc = dy / steps`
5. Start at (x1, y1). For each of the `steps + 1` points, plot `(round(x), round(y))` with `putpixel()`, then add the increments to `x` and `y`

The longer axis moves one pixel per step, and the other axis moves by a fraction, so the line stays continuous.

## Run

Run `dda.exe`, or compile `dda.cpp` with a compiler that has `graphics.h`. Enter the points when prompted:

```
Enter x1 y1: 100 100
Enter x2 y2: 300 200
```

A graphics window opens with the line drawn in white. Press any key to close it.

## Notes

- Uses floating-point increments and `round()`, which is simple but slower than integer-only methods like Bresenham's algorithm
- If both points are identical, `steps` is 0 and the program divides by zero. Entering two different points avoids this
