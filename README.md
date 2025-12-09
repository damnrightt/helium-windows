# kelle-browser-windows

Windows packaging for [Kelle Browser](https://github.com/damnrightt/helium).

## Credits

This repo is based on
[helium-windows](https://github.com/imputnet/helium-windows) and
[ungoogled-chromium-windows](https://github.com/ungoogled-software/ungoogled-chromium-windows).

## License
All code, patches, modified portions of imported code or patches, and
any other content that is unique to Kelle Browser and not imported from other
repositories is licensed under GPL-3.0. See [LICENSE](LICENSE).

## Building

### Setting up Visual Studio

[Follow the "Visual Studio" section of the official Windows build instructions](https://chromium.googlesource.com/chromium/src/+/refs/heads/main/docs/windows_build_instructions.md#visual-studio).

### Building Kelle Browser

Run in `Developer Command Prompt for VS` (as administrator):

```cmd
git clone --recurse-submodules https://github.com/damnrightt/helium-windows.git
cd helium-windows
python3 build.py
python3 package.py
```

A zip archive and an installer will be created under `build`.
