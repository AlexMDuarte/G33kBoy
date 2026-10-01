# G33kBoy

A Windows Game Boy emulator for DMG and Game Boy Color, built with C#/.NET and Avalonia.

## Features

- Load user-provided `.gb` and `.gbc` ROMs, including ROMs inside `.zip` files.
- Emulate Game Boy DMG and Color modes, audio, save states, and screenshots.
- Keyboard controls and XInput gamepads (Xbox and compatible controllers).
- Pause/resume, reset, display and sound options.

No commercial games or copyrighted ROMs are included. Use ROMs you are authorized to use.

## Controls

| Action | Keyboard | XInput gamepad |
| --- | --- | --- |
| Directions | Arrow keys | D-pad or left stick |
| A / B | X / Z | A / B |
| Select | Space | View / Back |
| Start | Enter | Menu / Start |
| Pause / resume | F6 | — |
| Reset | Ctrl+R | — |
| Open ROM | Ctrl+O | — |

Gamepad mapping is automatic and fixed. XInput controllers are polled by the emulator while it is open.

## Run on Windows

Download the `G33kBoy-Windows-x64.zip` release, extract it, and run `G33kBoy.exe`. Use **File > Open** or Ctrl+O to select your own ROM.

## Build from source

Requirements: .NET 10 SDK and Windows x64 for the packaged desktop application.

```powershell
dotnet build G33kBoy.sln -c Release
dotnet test UnitTests/UnitTests.csproj -c Release
```

The main application project is `G33kBoy/G33kBoy/G33kBoy.csproj`. NuGet packages restore during the build. See `THIRD-PARTY-NOTICES.txt` for dependency notices and licenses.

## License

The project is distributed under the MIT License. See `LICENSE` and the individual third-party license notices.
