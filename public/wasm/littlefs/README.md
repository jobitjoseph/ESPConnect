## LittleFS WASM drop-in

This folder is reserved for the LittleFS WebAssembly runtime that powers the SPIFFS/LittleFS tooling.

Place the vendor files you receive here using the following names:

```
public/wasm/littlefs/index.js
public/wasm/littlefs/index.d.ts
public/wasm/littlefs/littlefs.wasm
```

These files are ignored by Git (see the root `.gitignore`). Keeping them outside of source control allows you to use the proprietary or platform-specific build provided by your toolchain without accidentally committing it. The Vite dev server and production build will still be able to load the module from this path via the `public/` directory.
