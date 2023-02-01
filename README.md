# material-atomic-desgin-folder-icons

Material icons for atomic design folder structure

## Customize vscode folder icon for atomic design

1. Download icon files from `assets/icons` and move them to `(vscode-extensions-dir)/icons`.

   ex: `~/.vscode/extensions/icons/folder...svg`. Its' **NOT** your project vscode directory.

2. Add `PKief.material-icon-theme` extension and set as icon theme.

3. Open your User settings file. (Open vscode command pallet and input `>Preferences: Open User Settings`)

4. Add settings as below.

```
{
    (...other settings)
    "material-icon-theme.folders.associations": {
        "atoms": "../../../../icons/folder-atomic-design-atoms",
        "molecules": "../../../../icons/folder-atomic-design-molecules",
        "organisms": "../../../../icons/folder-atomic-design-organisms",
        "templates": "../../../../icons/folder-atomic-design-templates",
        "pages": "../../../../icons/folder-atomic-design-pages"
    }
}
```

5. Create folder for atomic design structure.
   <img src="https://raw.githubusercontent.com/gooodev/material-atomic-desgin-folder-icons/assets/readme/folder.png" alt="screenshot of vscode file explorer">

- If it doesn't work, check your material icon extension color setting and turn it to default. (This extensions customization doesn't work on other than default.)
  <img src="https://raw.githubusercontent.com/gooodev/material-atomic-desgin-folder-icons/assets/readme/change-color.png" alt="screenshot of changing extensions color">
