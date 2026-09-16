# build-plugin-nsjson

Test fixture for [nsis-dev/build-plugin](https://github.com/nsis-dev/build-plugin).

**Covers:** An unmigrated upstream. Several C files and a `.rc`, listed one by one (newline separated) to leave out the bundled `pluginapi.c` and the `ConsoleApp/`s. The bundled `pluginapi.h` still shadows the action's. The `.rc` is UTF-16LE, which MSVC `rc` reads and `windres` does not, so the mingw job is expected to fail.

**Changed from upstream:** Nothing in `Contrib/`; prebuilt `.exe`s removed from `Examples/`.
