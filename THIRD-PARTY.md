# Open-source components

AxeStation uses Qt for Python/PySide6 and Shiboken6 under LGPL v3, Qt runtime
libraries under their applicable LGPL v3 and permissive terms, zeroconf under
LGPL v2.1 or later, and certifi under MPL 2.0. Other components retain the licenses
listed below. The original application remains proprietary; third-party license
rights remain unchanged.

Complete notices are in [licenses](licenses/) and inside every app download.

| Component | Source / license |
| --- | --- |
| Qt 6.11.2: qtbase, qtdeclarative, qtsvg | LGPL v3 and component-specific permissive notices; full module sources below. |
| PySide6 and Shiboken6 6.11.2 | LGPL v3; full pyside-setup sources below. |
| zeroconf 0.154.0 | LGPL v2.1 or later. |
| certifi 2026.10.23 | MPL 2.0. |
| CPython 3.13.17 | Python Software Foundation and included notices. |
| ReportLab 5.1.0 | BSD-style. |
| Pillow 13.0.0 | MIT-CMU and included notices. |
| ifaddr 0.2.0 | MIT. |
| cryptography 50.0.2 | Apache 2.0 or BSD 3-Clause, with bundled OpenSSL notices. |
| cffi 2.1.1; pycparser 3.12 | MIT / BSD-style and included notices. |
| PyInstaller 6.22.3 bootloader | GPL v2 or later with bootloader distribution exception. |
| Inter and Roboto Mono fonts | SIL Open Font License 1.1, unmodified. |

## Corresponding library sources

[Download the third-party source bundle](https://github.com/SoloSatoshi/AxeStation-Downloads/releases/download/v1.4.0/AxeStation-Third-Party-Sources.zip).
The [source manifest](open-source/sources.json) lists exact upstream versions,
URLs, filenames, sizes and SHA-256 checksums. The bundle includes complete,
unmodified upstream archives for the Qt modules, Qt for Python, Python runtime
and Python libraries used by this release. Font files and licenses are included.

The application dynamically links these libraries. LGPL-covered Python modules
are also supplied as replaceable files. Users may modify or replace the LGPL
components and reverse engineer the application as needed to debug those
modifications. See [library replacement instructions](open-source/REPLACING-LIBRARIES.md).

Library modifications can affect device communication, report accuracy and
stability. Solo Satoshi's official checksums apply to the unmodified downloads.
No source access to the proprietary application is required to exercise rights
granted for its third-party components.
