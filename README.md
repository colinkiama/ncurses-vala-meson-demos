# ncurses-vala-meson-demos

Rebuilding the [existing ncurses vala demos](https://github.com/kucaahbe/ncurses.vala) with more modern build tooling

## Prerequisites

```
libncurses
valac
```

## Building

```bash
meson build --prefix=/usr
cd build
ninja
```

All the demos will be available in the `build` of the project e.g `build/src/<program_name>`.
