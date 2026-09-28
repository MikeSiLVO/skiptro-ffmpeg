# skiptro-ffmpeg

Unmodified FFmpeg builds bundled with [Skiptro](https://github.com/MikeSiLVO/skiptro-releases). Every
Skiptro release downloads them from here, so all platforms ship the same FFmpeg version. Each file is
the builder's own archive, renamed. Checksums matched the builder's published checksums when mirrored.

## 9.0.2

| File | Builder | Original build |
|---|---|---|
| `ffmpeg-9.0.2-win64.zip` | BtbN | `ffmpeg-n9.0.2-14-gebafaee10a-win64-gpl-9.0.zip` |
| `ffmpeg-9.0.2-linux64.tar.xz` | BtbN | `ffmpeg-n9.0.2-14-gebafaee10a-linux64-gpl-9.0.tar.xz` |
| `ffmpeg-9.0.2-linuxarm64.tar.xz` | BtbN | `ffmpeg-n9.0.2-14-gebafaee10a-linuxarm64-gpl-9.0.tar.xz` |
| `ffmpeg-9.0.2-macos-amd64.zip`, `ffprobe-9.0.2-macos-amd64.zip` | Martin Riedl | build `1789931006_9.0.2` |
| `ffmpeg-9.0.2-macos-arm64.zip`, `ffprobe-9.0.2-macos-arm64.zip` | Martin Riedl | build `1789931890_9.0.2` |

The BtbN files come from release `autobuild-2026-09-28-13-06`. `SHA256SUMS` in the release lists
every file.

## License and source

These builds enable GPL components, so FFmpeg is licensed to you under the GNU General Public License
version 3. The full text is in [COPYING](COPYING).

Source code for these builds:

- FFmpeg: https://git.ffmpeg.org/ffmpeg.git at commit `ebafaee10a` (BtbN builds) and tag `n9.0.2`
  (macOS builds)
- BtbN build recipe: https://github.com/BtbN/FFmpeg-Builds/tree/16523e260106182950d7072b6ea1401808f68a50.
  Each script in `scripts.d` pins its library to an exact repository and commit.
- Martin Riedl build script: https://git.martin-riedl.de/ffmpeg/build-script. Library versions for
  each build: `https://ffmpeg.martin-riedl.de/download/macos/<arch>/<build>/versions.txt`
