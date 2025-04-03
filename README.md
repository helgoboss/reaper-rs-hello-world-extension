# reaper-rs-hello-world-extension

This is a minimal REAPER extension built using [reaper-rs](https://github.com/helgoboss/reaper-rs). As per official recommendation, 
it uses the medium-level API only (which unlike the high-level API is quite stable and mature).

## Build

1. [Install latest stable Rust](https://www.rust-lang.org/)
2. Run `cargo build`
3. Copy `target/debug/libreaper_rs_hello_world_extension.dylib` to `$REAPER_RESOURCE_DIR/UserPlugins/reaper_rs_hello_world_extension.dylib`
   - This is assuming macOS. On Windows, the extension is `dll` and on Linux it's `so`. 
   - Or create a symbolic link so you don't have to copy it again after each build.
   - Make sure to remove the `lib` prefix! Otherwise, REAPER won't load your extension.