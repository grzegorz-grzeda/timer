# timer

Simple timer utility for managing different time interval clients.

This is a [G2EPM](https://github.com/grzegorz-grzeda/g2epm) library.

## How to compile and link it?

Just include this directory in your CMake project.

You **MUST** specify:
- `TIMER_ENTRIES_MAX_COUNT` the maximum number of running timers,

Example `CMakeLists.txt` content:
```
...

add_subdirectory(<PATH TO THIS LIBRARY>)
target_compile_definitions(timer PRIVATE TIMER_ENTRIES_MAX_COUNT=20)
target_link_libraries(${PROJECT_NAME} PRIVATE timer)

...
```

# Copyright
This library was written by G2Labs Grzegorz Grzęda, and is distributed under MIT Licence. Check the `LICENSE` file for more details.