# build-plugin-nsjson

Test fixture for [nsis-dev/build-plugin](https://github.com/nsis-dev/build-plugin).

> [!CAUTION]
> This is not an official plugin repository.

**Covers:** An unmigrated upstream. Several C files and a `.rc`, listed one by one (newline separated) to leave out the bundled `pluginapi.c` and the `ConsoleApp/`s. The bundled `pluginapi.h` still shadows the action's.

**Changed from upstream:** For MinGW: `nsJSON.rc` and `resource.h` converted from UTF-16LE to UTF-8 (with `#pragma code_page(65001)`), `#include`s lowercased for case-sensitive headers, and two casts GCC rejects fixed. Prebuilt `.exe`s removed from `Examples/`.
