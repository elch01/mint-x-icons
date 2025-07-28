## Summary

This is a test repository to **identify and remove non-GPLv3-compliant icons** from the icon pack.

Mint-X-Icons is a fork of Faenza, and all icons in this repository are **intended to be GPLv3 licensed**.

However, many SVG files **lack proper Inkscape license metadata**, and the pack includes **trademarked icons** (e.g., Firefox, YouTube, Google) that cannot be GPL-licensed.

For clarity:
- **All original icons** (not containing trademarks) are assumed **GPLv3**.
- **Trademarked icons** are **not GPL-compliant** and must be **removed or replaced**.

## Goals

-  Identify and remove non-GPL-compliant icons
-  Add GPL license metadata to all `.svg` files
-  Ensure all remaining icons are fully GPLv3 compliant

## License Compatibility Overview for Icons

| License / Source              | GPL-Compatible?     | Action / Notes                                                                 |
|------------------------------|----------------------|--------------------------------------------------------------------------------|
| **GPLv3 / GPLv2**            | ✅ Yes               | Fully compatible. All original icons licensed under GPLv3.                     |
| **MIT / BSD (2/3-Clause)**   | ✅ Yes               | Can be used and relicensed as GPL.                                             |
| **Apache 2.0**               | ✅ Yes (GPLv3 only)  | Allowed in GPLv3 themes, not GPLv2.                                            |
| **CC0 (Public Domain)**      | ✅ Yes               | Can be relicensed under GPL.                                                  |
| **CC BY 4.0**                | ⚠️ Yes (with attribution) | Allowed with attribution; must be marked clearly.                              |
| **CC BY-SA 4.0**             | ⚠️ Limited           | May conflict with GPL. Best kept separate or used with caution.               |
| **CC BY-NC / BY-ND / NC-SA** | ❌ No                | Not GPL-compatible. Cannot be used.                                           |
| **MPL 2.0 (e.g., Firefox)**  | ⚠️ Yes (GPLv3 only)  | Combine only with GPLv3. Still subject to trademark restrictions.             |
| **Trademarked Logos**        | ❌ No                | Cannot be GPL-licensed. Must be removed or redesigned to avoid logo use.      |
| **Unknown License**          | ❌ No (until clarified) | Remove or create a GPL replacement until confirmed.                            |

## ⚠️ Note on Logos and Trademarks
Icons representing brands (e.g., Google, Facebook, LibreOffice, Firefox) are **not GPL-licensed**, even if the app is open source. These logos are **trademarked**, and in this repo should be **removed and replaced** with generic icons.

## Repository Structure
```
mint-x-icons/
├── LICENSE # GPLv3 license
├── README.md # This table + notes on trademarked icons
├── apps/ # Template, can probably be removed and the themplate placed elsewhere
├── usr/share/ # Icons
├── EXCEPTIONS.md # List of files with non-GPL status or special licenses, might not be needed.
├── create-links # automates symbolic link creation across various color-themed icon directories
├── create-symbolic-link-from-list.py # automates the bulk creation and cleanup of icon symbolic links 
├── deadlinks # Checks for dead symlinks
├── show-diffs # Compares Mint-X with Mint-Xtra (Local test directory, not a part of the repo)
├── symbolic-apps-list # Documentation
├── symbolic-categories-list # Documentation
├── test # Test the icon theme by removing the icons installed in /usr/share/icons/Mint-X* and readding data from the repo.
``` 

## Attribution / Licensing Metadata
All icons must include metadata where applicable, and GPL-licensed icons **must** clearly marked with license tags in the SVG files.

## License Attribution

This icon theme is a fork of the **Faenza Icon Theme** by **Matthieu James (Tiheum)**.

 Original Repository: [Google Code Archive – Faenza](https://code.google.com/archive/p/faenza-icon-theme/)  
 License: **GNU GPL v3**

Note: Original SVG files in Faenza lacked embedded license metadata, but the entire icon set is clearly licensed under GPLv3.

