# Jack's Jam Room app

The app players use to jam in [Jack's Jam Room](https://jacksjamroom.com) private rooms.

It is a build of **[Jamulus](https://github.com/jamulussoftware/jamulus)**, the free, open-source program for playing music
together live over the internet, written by Volker Fischer and the Jamulus contributors. All the credit for the jam engine
is theirs. The original project's README is in [README-JAMULUS.md](README-JAMULUS.md).

## What this build changes
- The name **Jack's Jam Room** in the window title, dialogs and installer, and its own settings folder.
- Jack's icon for the app, window and installer.
- The Windows installer installs into its own folder with its own Start menu and uninstall entries, so it sits beside an
  official Jamulus install and never removes one.
- The About box credits Jamulus and links this source code.

The jam engine and network protocol are unchanged: it works with any Jamulus server, Jack's private rooms included.
Based on Jamulus 3.12.6 (upstream commit b2bf22e0d329a43dd222749737df244b8fc3b16e).

## Download
Windows: the latest installer is on the [Releases](../../releases/latest) page. Mac and Linux players use the official
Jamulus download from [jamulus.app](https://jamulus.app/).

## Building
Every push to `main` builds the Windows installer with GitHub Actions (`.github/workflows/build-windows.yml`, using
Jamulus's own build scripts). A tag starting with `v` also publishes it as a release. See [COMPILING.md](COMPILING.md) to
build it yourself.

## Licence
Jamulus is licensed under the GNU Affero General Public License 3.0 or later (code contributed before 3.12.1dev: GPL 3.0 or
later). This build is distributed under the same terms; see [COPYING](COPYING). The changes listed above are the only
differences from upstream Jamulus 3.12.6, and their full source is in this repository.

Jamulus is the Jamulus project's name; this build is not made or endorsed by the Jamulus project.
