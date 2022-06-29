# reaper-rs-hello-world-extension

This is a minimal REAPER extension built using [reaper-rs](https://github.com/helgoboss/reaper-rs). It uses a small part of the (currently unstable) high-level API of reaper-rs to boostrap the plug-in and then immediately goes down one level to the much more stable medium-level API.

## Build

1. [Install latest stable Rust](https://www.rust-lang.org/)
2. Run `cargo build`
1. Copy `target/debug/libreaper_rs_hello_world_extension.dylib` to `$REAPER_RESOURCE_DIR/UserPlugins/reaper_rs_hello_world_extension.dylib`
   - Or create a symbolic link so you don't have to copy it again after each build.
   - Make sure to remove the `lib` prefix! Otherwise, REAPER won't load your extension.