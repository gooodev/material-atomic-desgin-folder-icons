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

5. Create folders for atomic design structure.
<img src="https://github.com/gooodev/material-atomic-desgin-folder-icons/blob/main/assets/readme/folder.png" alt="screenshot of vscode file explorer">

### If it doesn't work, please check below
- Icon paths have to be the relative path from "dist" folder of extension. Please check below for detail.
https://github.com/PKief/vscode-material-icon-theme/issues/1834
- If it doesn't work, check your material icon extension's color setting and turn it to default. (This folder icon association setting doesn't work with custom color setting.)
<img src="https://github.com/gooodev/material-atomic-desgin-folder-icons/blob/main/assets/readme/change-color.png" alt="screenshot of changing extensions color">
