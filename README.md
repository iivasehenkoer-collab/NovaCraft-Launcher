# NovaWin 10 Lite

Сборщик загрузочного ISO Windows 10 x64 для Intel Core i7-9750H, NVIDIA GTX 1650 и 16 GB RAM.

**Проект и исходники:** [NovaWin10Lite_1.0.0_Source.zip](NovaWin10Lite_1.0.0_Source.zip)

Архив содержит PowerShell-скрипт сборки bootable ISO (BIOS + UEFI), сценарии первого запуска Windows, автоматическую установку Firefox, Steam, Telegram Desktop и WinRAR через WinGet, загрузку/запуск Sota VPN и безопасные игровые настройки.

## Важно

- Это набор для локальной сборки, а не готовый ISO: оригинальный Windows 10 ISO нужно скачать у Microsoft.
- Для сборки нужен Windows ADK с компонентом Deployment Tools (`oscdimg.exe`).
- ISO создаётся локально. В репозитории не распространяются установочные файлы Windows.
- Windows Defender, Windows Update, Firewall, драйверы и системные компоненты не отключаются.
- Edge остаётся системным компонентом; после установки Firefox нужно выбрать его браузером по умолчанию в настройках Windows.
- Установщик Sota VPN открывается обычным мастером, так как тихий ключ запуска не подтверждён.

См. подробную инструкцию внутри ZIP в файле `README.md`.
