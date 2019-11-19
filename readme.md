# Build the 32 bit Java Access Bridge for Windows using SCons

The NVDA screen reader is a 32 bit application and requires the 32 bit Java Access Bridge client dll.
This will happily talk to 64 bit Java applications.
However, since Java 10, 32 bit builds are no longer provided.
This repository contains an SConstruct to build just the 32 bit Java Access Bridge from the OpenJDK source code using SCons.

## Instructions

1. Install Microsoft Visual Studio 2017 Community.
2. Install SCons version 3.0 or later.
3. Clone this repository:

    `git clone https://github.com/jcsteh/javaAccessBridge32.git`

4. Fetch the OpenJDk Git submodule:

    `git submodule update --init`

5. Assuming scons is in your path, simply run:

    `scons`

    The dll will be built as `build\WindowsAccessBridge-32.dll`.
