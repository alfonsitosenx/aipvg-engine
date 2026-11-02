# AI Product Video Generator: server video engine

This repository hosts the optional **server video engine** used by
[AI Product Video Generator Pro](https://excesspronet.com) (Excess Pro Net LLC). The plugin uses it to
make light product videos on the server, so shop owners do not have to keep a browser tab open.

The release files are **unchanged static Linux builds of ffmpeg 7.0.2** by John Van Sickle
(<https://johnvansickle.com/ffmpeg/>), repackaged as ZIP files so WordPress can unpack them without
extra tools. Each ZIP holds `ffmpeg`, its build information and the GPLv3 licence.

| File | CPU | SHA-256 |
|---|---|---|
| `aipvg-engine-ffmpeg-7.0.2-linux-amd64.zip` | x86_64 | `f1b03587205bfccdf369feef68aaeba0a79ff848df91344d09534a8e39a6d657` |
| `aipvg-engine-ffmpeg-7.0.2-linux-arm64.zip` | aarch64 | `c0c61108d2d95caab770d5c19099760c33cfa0561fb3ff4b0bd3ad33e9d08f4f` |

The plugin refuses any download whose SHA-256 differs from the value built into it.

The original archives were checked against the MD5 sums John Van Sickle publishes
(`7fa72b652e19bf84c9461e332ea1cdf3` amd64, `807afe21601db0a73e426121c7d636ea` arm64) before repackaging.

## Licence and source

ffmpeg is licensed under the GNU General Public License version 3 (`LICENSE-ffmpeg-GPLv3.txt`).
Its complete source code is available at <https://ffmpeg.org/releases/ffmpeg-7.0.2.tar.xz>, and the
build configuration is listed in `BUILD-INFO.txt` inside each ZIP.
