# Dear ImGui software renderer
This is a software renderer for [Dear ImGui](https://github.com/ocornut/imgui).
I built it not out of a specific need, but because it was fun.
The goal was to get something accurate and decently fast in not too many lines of code.
It renders a complex GUI in 1-10 milliseconds on a modern laptop.

# How to use:
Just copy `imgui_sw.hpp` and `imgui_sw.cpp`. There are no other dependencies beside Dear ImGui.

# Example:
This renders in 7 ms on my MacBook Pro:

![Software rendered](screenshots/imgui_sw.png)

# Future work:
* We do not yet support painting with any other texture than the default font texture.
* Optimize rendering of gradient rectangles (common for color pickers)

# How to test it
```
git clone https://github.com/emilk/imgui_software_renderer.git
cd imgui_software_renderer
git submodule update --init --recursive
./build_and_run.sh
```

# License:
This software is dual-licensed to the public domain and under the following
license: you are granted a perpetual, irrevocable license to copy, modify,
publish, and distribute this file as you see fit.
