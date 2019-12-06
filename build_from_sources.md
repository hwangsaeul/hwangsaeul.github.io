## Getting Started

### Install meson and ninja
Meson 0.40 and newer is required.

### Build module
You can get library and executables built running:
```
meson build
ninja -C build
```

#### Install

```
ninja -C build install
```

#### Compile gschema

```
glib-compile-schemas /usr/local/share/glib-2.0/schemas/
```
