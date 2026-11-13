# Replacing open-source libraries

Use a separate copy of the application for library development. Close it before
replacing files. Keep the original download so you can restore it.

## Windows

Extract the entire official ZIP into a writable folder. Shared libraries and
replaceable Python packages are in `AxeStation/_internal/`. Qt DLLs and plugins
are under the included PySide6 runtime folders. Replace a library or package
with a compatible build for the same Windows x64 architecture, Python ABI and
Qt/PySide version. Keep the folder structure and required dependencies together.

## macOS

Copy `AxeStation.app` into a writable development folder. In Finder, choose
**Show Package Contents**. Shared frameworks and replaceable Python modules live
in `Contents/Frameworks` and `Contents/Resources`, with internal links between
those locations. Preserve the links when replacing files. Builds must target
Apple Silicon and match the included Python ABI and Qt/PySide version.

Changing a signed bundle invalidates its signature. After replacing libraries,
you can apply a local ad-hoc signature to your development copy:

```sh
codesign --force --deep --sign - AxeStation.app
```

This signs your local copy; it does not make it an official Solo Satoshi build or
bypass operating-system permissions.

## Sources and licenses

The [source manifest](sources.json) and release source bundle provide complete
upstream sources. Follow each upstream project's build instructions and preserve
its license notices. Qt/PySide, zeroconf and other components retain their own
license rights. The original application license expressly preserves LGPL library
replacement and the reverse engineering needed to debug those modifications.

In-app updates replace the application and its libraries with an official build.
Keep your modified development copy separately if you want to retain changes.
