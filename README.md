# NovaCraft Launcher

NovaCraft is a planned Windows launcher for Minecraft: Java Edition, with a dark gaming interface and blue-crystal **N** branding.

> **Project status: planning / implementation in progress.** This repository currently contains project documentation only. It does not yet contain a working launcher, installer, or release ZIP.

## Planned experience

- Minecraft-style home dashboard with version selection and a prominent Play action
- Installations and profile management
- Local guest profiles (launcher identity only; not Minecraft authentication)
- Microsoft account authentication through supported official flows
- Mods and modpacks discovery through the official Modrinth API
- Fabric, Forge, and NeoForge compatibility filtering
- Performance center for RAM and Java configuration
- Java installation assistance
- Skin Studio for importing, previewing, and exporting valid Java skin PNGs
- Theme store, crash log viewer, gaming statistics, and update center
- YouTube page that opens the official YouTube website, with a browser fallback
- NovaCraft loading screen and blue-crystal N branding

## Minecraft and authentication

NovaCraft is intended to launch Minecraft: Java Edition through **Legacy Launcher** where supported. The launcher must clearly disclose any external dependency and must not bundle or redistribute Legacy Launcher or Minecraft unless their licences and distribution terms permit it.

Local guest profiles are only local launcher profiles. They do not authenticate with Microsoft, grant ownership of Minecraft, or provide access to online-mode servers. Authentication must use supported official flows. This project will not distribute cracked game files or bypass authentication.

## Development status

Features listed above are planned requirements, not claims that they are already implemented. A release will be published only after the application is built and tested.

## Contributing

Issues and pull requests are welcome. Please describe reproducible bugs, expected behaviour, and your environment.

## License

No project license has been selected yet. Until a license is added, the source (when published) is not granted an open-source license by this repository.
