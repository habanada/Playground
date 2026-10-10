# NimbusForms

**A renderer-first, GDI+-powered UI component suite for Delphi VCL.**

**Personal project · Work in progress · Highly experimental**

![NimbusForms VCL demo in dark mode](docs/screenshots/overview.jpg)

NimbusForms is my Delphi/VCL port of **my own C# WinForms UI library**. The C# version is my project too; this is not a port of somebody else's work.

The idea is to bring the same approach to Delphi: modern-looking, theme-aware desktop controls built around **custom drawing and a reusable rendering layer**, instead of simply putting a new skin on standard Windows controls.

This is a long-running personal project. A lot has been implemented, but **very little has been thoroughly tested**.

> [!CAUTION]
> **Not production-ready.** NimbusForms is still in heavy development. Expect unfinished features, bugs, rendering issues, breaking API changes and rough edges. The screenshots demonstrate what is currently being worked on, not a promise that every component is stable.

## Renderer-first by design

Rendering is the foundation of NimbusForms, not an afterthought.

- **Custom GDI+ drawing:** controls are designed and painted with their own visuals, rather than relying on default Windows control rendering.
- **Reusable rendering approach:** shared drawing, styling and layout concepts provide a consistent foundation for different controls.
- **Theme-aware UI:** dark/light themes, accent colors, semantic colors and custom visual states.
- **DPI-aware design:** scaling, measurements and rendering are considered throughout the component work.
- **VCL integration:** custom-drawn surfaces where they matter, with native VCL functionality retained where it makes sense.

The goal is a coherent component suite, not just a collection of separately styled widgets.

## What's in the demo?

| Area | Controls and features shown |
| --- | --- |
| **Window and layout** | Themed forms, custom title bars, window states, snap-layout experiments, split containers |
| **Navigation** | Tab controls, menu bars, toolbars, breadcrumb bars, tree views, step indicators |
| **Data and editors** | Virtual list view, hex editor, date/time picker, date-range picker |
| **Inputs** | Buttons, checkboxes, toggles, radio buttons, combo boxes, sliders, range sliders, tag input |
| **Visuals** | Color pickers, palette selection, styled labels with lightweight markup, progress indicators, badges and avatars |

Some parts are much further along than others. Inclusion here means **visible in the current demo**, not finished or fully tested.

### Hex editor with a piece table

The hex editor uses a **piece-table-based editing approach**. That is one of the more interesting parts of the project, but it is also under active development and should be considered experimental.

### Virtual list view

The virtual list view is designed around on-demand row data instead of creating a VCL control for each item. The demo shows a **100,000-row example**, including columns, grouping and expandable details. This is a demo scenario, not a benchmark or a performance guarantee.

## Screenshots

### Dates, editors and large data sets

| Date and time picker | Multi-month date-range picker |
| :---: | :---: |
| ![Date and time picker](docs/screenshots/date-picker.jpg) | ![Date-range picker with presets](docs/screenshots/date-range-picker.jpg) |

| Piece-table hex editor | Virtual list view |
| :---: | :---: |
| ![Hex editor](docs/screenshots/hex-editor.jpg) | ![Virtual list view](docs/screenshots/virtual-list-view.jpg) |

### Controls and rendering

| Color picker | Tree view |
| :---: | :---: |
| ![Color picker and palette controls](docs/screenshots/color-picker.jpg) | ![Themed tree view](docs/screenshots/tree-view.jpg) |

| Toolbars | Menus |
| :---: | :---: |
| ![Themed toolbar](docs/screenshots/tool-bar.jpg) | ![Themed menu bar](docs/screenshots/menu-bar.jpg) |

| Tag input | Step indicator |
| :---: | :---: |
| ![Tag input variants](docs/screenshots/tag-input.jpg) | ![Step indicator variants](docs/screenshots/step-indicator.jpg) |

| Styled label / mini markup | Split containers |
| :---: | :---: |
| ![Styled label renderer](docs/screenshots/styled-label.jpg) | ![Split container layout](docs/screenshots/split-container.jpg) |

### Custom window chrome

| Themed form | Window states and title bar |
| :---: | :---: |
| ![Custom themed form](docs/screenshots/themed-form.jpg) | ![Themed form states](docs/screenshots/themed-form-states.jpg) |

![Windows snap-layout experiment](docs/screenshots/snap-layouts.jpg)

## Project status

**Early / experimental.** This repository documents an ongoing port and rewrite, not a finished framework release.

- Components and APIs may be incomplete or change without notice.
- Rendering and behavior are not comprehensively tested across environments, themes or DPI settings.
- Bugs, edge cases and unfinished interactions are to be expected.
- There is currently no promise of a stable release schedule or production support.

I have been working on NimbusForms for a long time. The main reason the Delphi port takes time is simple: **porting an entire GUI library from C# is a lot of work**, and some days I would rather keep building the C# version than translate another component. Both codebases are mine, and both matter to me.

This project will keep evolving as time and motivation allow.

## Using NimbusForms

For now, treat this as **development-stage source and a component showcase**. The screenshots come from the VCL demo application; they are not a substitute for testing in your own environment. Setup requirements, supported Delphi versions and a stable public API have not yet been documented here.

If you're exploring the code, expect things to move around while the renderer and components evolve.

---

**Built from scratch, drawn with GDI+, and still very much under construction.**
