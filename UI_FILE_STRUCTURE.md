# Blockscout UI File Inventory

This document provides a map of the UI-related files and directories for the Amero X Explorer (Blockscout).

## 1. HTML Templates (Phoenix/EEX)
These files define the structure and content of the pages.
- **Location**: `apps/block_scout_web/lib/block_scout_web/templates/`
- **Key Files**:
  - `layout/app.html.eex`: The main wrapper (header, footer, meta tags). This is where the root layout lives.
  - `chain/show.html.eex`: The dashboard/home page.
  - `address/show.html.eex`: Individual address page.
  - `transaction/show.html.eex`: Transaction details page.
  - `block/show.html.eex`: Block details page.

## 2. Stylesheets (SCSS / CSS)
Blockscout uses Sass for styling.
- **Location**: `apps/block_scout_web/assets/css/`
- **Key Files**:
  - `app.scss`: Main entry point for styles.
  - `theme/_amero_variables.scss`: (Your custom file) Contains brand colors and variables for Amero X.
  - `theme/`: Directory containing specific theme overrides (dark mode, light mode).

## 3. Brand Assets (Images, Icons, Logos)
- **Location**: `apps/block_scout_web/assets/static/images/`
- **Key Files**:
  - `amero_x_logo.png`: Your custom network logo.
  - `favicon.ico`: The site favicon.
  - `blockscout_logo.png`: Original Blockscout branding.

## 4. UI Logic (Views)
Views in Phoenix handle data formatting for the templates. 
- **Location**: `apps/block_scout_web/lib/block_scout_web/views/`
- **Key Files**:
  - `layout_view.ex`: Logic for the header/footer and global site variables.
  - `block_view.ex`: Formatting for block numbers, timestamps, etc.
  - `transaction_view.ex`: Formatting for hex data and gas values.

## 5. JavaScript (Frontend Logic)
- **Location**: `apps/block_scout_web/assets/js/`
- **Key Files**:
  - `app.js`: Root JS file.
  - `lib/`: Scripts for charts, search autocomplete, and socket connections.

## 6. LiveView (Interactive Components)
More recent versions of Blockscout use LiveView for real-time updates.
- **Location**: `apps/block_scout_web/lib/block_scout_web/live/`
