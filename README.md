# BIMLens

Live BIM data dashboards for Autodesk Revit 2024, 2025 and 2026.

The dashboard runs in your browser at **https://ibrahimfahdah.github.io/BIMLens/** and talks to a small Revit add-in on your own machine. Model data stays on your computer: the add-in only listens on `127.0.0.1`.

## Install

1. Download the zip for your Revit version from [Releases](../../releases).
2. Close Revit, unzip, and run `install.ps1` (right-click → Run with PowerShell).
3. Start Revit, open a model and click **BIMLens** on the ribbon. The dashboard opens in your browser.

## Requirements

- Chrome or Edge. The first time, the browser asks to allow access to devices on your local network: choose **Allow**, that is the connection to Revit.
- Firefox and Safari block a hosted page from calling the local add-in.

## Working offline

The zip also contains a copy of the dashboard. Delete `weburl.txt` from `%AppData%\Autodesk\Revit\Addins\<year>\BIMLens\` and the add-in opens that copy instead.
