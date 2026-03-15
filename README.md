# Display Control+

Display Control+ is a Windows desktop utility designed to protect OLED and other sensitive displays during idle time while still allowing a branded or customized screen experience.

## What It Does

Instead of relying on a single black screen or a generic screen saver, Display Control+ lets you apply monitor-aware idle overlays using:

- Solid black protection mode
- Single-image overlays
- GIF overlays
- Slideshow overlays

The app runs with a GUI plus a background overlay service, allowing users to configure settings once and keep protection active after logon.

## Current Use Case

This project is best positioned as a desktop productivity and display-protection tool for:

- OLED monitor owners
- multi-monitor workstation setups
- always-on desk setups
- streamers, developers, and power users who leave screens idle for long periods

## Core Features

- Per-monitor monitor selection
- System-wide or per-monitor idle detection
- Multiple idle detection modes: input, activity, or both
- Preview before applying settings
- Background service startup after configuration
- Install-on-startup flow via scheduled task helper
- Packaging scripts for executable and installer generation
- Test scripts for overlay, idle, workflow, and end-to-end behavior

## Technical Notes

The repository currently includes:

- Main GUI application in `main.py`
- Overlay rendering logic in `overlay.py` and `overlay_bg.py`
- Activity detection and monitoring logic in `monitor_activity.py` and `monitor_control.py`
- Update/version support in `update_manager.py`
- Build and packaging scripts for Windows distribution
- Installer and release preparation assets

## Business Value

Display Control+ demonstrates Knight Logics capability in:

- Windows desktop application development
- background process orchestration
- system integration and startup automation
- user-focused utility tooling
- packaging Python applications into distributable executables

This makes it a strong GitHub and Upwork case study for custom desktop tooling.

## Installation

### Option 1: Release Build

Download the latest packaged release from the Releases page and run the installer or bundled executable.

Releases: https://github.com/Knight-Logics/Display-Control/releases

### Option 2: Run From Source

1. Clone the repository
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the application:

```bash
python main.py
```

## Typical Workflow

1. Launch the app
2. Select which monitors to protect
3. Choose protection mode: black, image, slideshow, or GIF
4. Configure idle timeout and detection scope
5. Preview overlay behavior
6. Apply settings and enable background protection
7. Optionally install startup task for automatic logon behavior

## Status

Operational and usable today. The product can still be refined further, but the current implementation is already a credible proof of desktop utility design, background automation, and Windows packaging.

## License

MIT