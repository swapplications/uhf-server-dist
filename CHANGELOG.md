# UHF Server - Changelog

## 1.6.0

- Added support for recurring recordings (requires UHF 1.87.0).
- Improved retry mechanism and added support for more video formats.

## 1.5.1

- More HLS compatibility fixes.

## 1.5.0

- Fixed the recording of HLS and DASH streams.
- Improved the logging of ffmpeg errors.
- Made a Docker image available in Docker Hub (`swapplications/uhf-server`) and improved the Dockerfile.
- The GUI now offers a quick access to the logs file from the contextual menu of the status bar app.

## 1.4.0

- UHF Server can now detect commercials. Set the `--enable-commercial-detection` argument when invoking the
command line tool or enable the commercial detection checkbox in the macOS or Windows GUI. This commercial 
detection takes place when a scheduled recording finishes and it can take several minutes to complete. This
functionality is compatible with UHF 1.67.0 (iOS) and 1.55.0 (tvOS).

## 1.3.0

- The GUI for Windows and macOS now includes an option to automatically launch the server at system startup.
- Improved error reporting when starting the server in the Windows and macOS apps.
- The server now starts automatically when launching the Windows and macOS apps.
- Recordings now use the program name and date as the file name.
- Fixed a performance issue in the server that caused degraded performance when multiple recordings finished.

## 1.2.0

- The GUI for Windows and macOS now display the IP address the server is running on.
- The GUI now informs about new updates available.
- Prevented FFmpeg from opening a blank window in Windows while recording.
- Prevented machine from going idle while the server is running.
- Fixed detection of FFmpeg errors.
- Fixed error notifications.
- Improved ffmpeg retry logic.

## 1.1.0

- Fixed macOS permissions issue.
- Improved performance while recording a stream.

## 1.0.0

- Initial release.
- Configurable recordings directory, port and server password.
- GUI compatibility: macOS arm64, Windows x64.
- CLI compatibility: Linux x64, Linux arm64.
