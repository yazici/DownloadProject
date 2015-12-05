# DownloadProject

This repository contains a generalized implementation for downloading an
external project's source at CMake's configure step rather than as part
of the main build. The primary advantage of this is that the project's source
code can then be included directly in the main CMake build using the
add_subdirectory() command, making all of the external project's targets,
etc. available without any further effort. The technique is fully explained
in the article available at:

http://crascit.com/2015/07/25/cmake-gtest/

An example as described in that article is provided here to demonstrate
how to use the DownloadProject module. It uses [googletest][1] as the
example, downloading and building trivial gtest and gmock test cases
to show the technique.

[1]: https://github.com/google/googletest
