# Extraction Workflow

Use fast static inspection. Prefer `rg`/`rg --files`, archive listings, and text extraction from CSS/PHP metadata. Do not execute theme code.

## Inventory

Useful counts:

```powershell
Get-ChildItem -Recurse -File | Group-Object Extension | Sort-Object Count -Descending
Get-ChildItem -Recurse -File -Filter *.zip | Measure-Object
Get-ChildItem -Recurse -Filter style.css -File
```

For ZIP internals on PowerShell:

```powershell
Add-Type -AssemblyName System.IO.Compression.FileSystem
$zip = [System.IO.Compression.ZipFile]::OpenRead($path)
$zip.Entries | Select-Object FullName, Length
$zip.Dispose()
```

## Theme-Like Signals

Count a ZIP or folder as theme-like when it contains several of:

- `style.css`
- `functions.php`
- `header.php`
- `footer.php`
- `front-page.php` or `frontpage/`
- `screenshot.png`
- `customizer/` or `inc/customizer`
- `templates/`
- `woocommerce.php`

## CSS Signals

Extract:

- Theme header fields: `Theme Name`, `Description`, `Tags`, `Template`, `Version`.
- Repeated class selectors.
- Color tokens and neutral/action balance.
- Responsive breakpoints.
- Component names: `header`, `slider`, `service`, `portfolio`, `team`, `testimonial`, `product`, `footer`.

Interpret classes as design evidence, not code to reuse.

## PHP/Template Signals

Look for:

- Header variants such as `head-type1.php`.
- Slider variants such as `slider-static.php`, `slider-customslider.php`, `slider.php`.
- Front-page option panels such as `settings-frontpage.php`.
- Contact templates, blog templates, page builder templates, sidebar variants.
- Widget areas and menus.

## Suggested Report

```markdown
# Theme Corpus Analysis

## Corpus
- Path:
- Archives:
- Extracted themes:
- Theme-like packages:
- Plugin packages:

## Repeated Architecture
- Header:
- Hero/slider:
- Front-page sections:
- Commerce:
- Customizer/options:

## Visual Patterns
- Layout:
- Typography:
- Color:
- Imagery:
- Components:

## Transferable Design Rules
1.
2.
3.

## Do Not Copy
- Vendor code:
- Images/demo data:
- Bundled plugins:
```

## Red Flags

- Bundled third-party dependencies with tests or old packages.
- Payment plugins or API integrations.
- Minified scripts where source is unclear.
- License files that do not allow redistribution.
- Demo assets that look proprietary.
