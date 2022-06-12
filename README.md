# Metro for Steam with Unofficial Patch skin

This merges the [Metro for Steam skin](https://github.com/minischetti/metro-for-steam) with the [Unofficial Patch](https://github.com/redsigma/UPMetroSkin/).

### Install Instructions

##### Manual updating

Download Latest [release](https://github.com/SaltireSoul/SteamMetroSkin/archive/refs/heads/master.zip)

- Extract/Copy metro-for-steam into your SteamDir/skins/ folder
  - on Windows this should be `C:\Program Files (x86)\Steam\skins`

##### Git

> From within SteamDir/skins/ folder via terminal

*Required*: `git config --global --add safe.directory "C:/Program Files (x86)/Steam/skins"`

- Tidy version (only fetches metro-for-steam directory)
  
  ```bash
  git init
  git remote add -f origin https://github.com/SaltireSoul/SteamMetroSkin.git
  git config core.sparseCheckout true
  echo metro-for-steam >> .git/info/sparse-checkout
  
  ## Download with pull, not clone
  git pull origin master
  ```

- Messy version
  
  ```bash
  git clone https://github.com/SaltireSoul/SteamMetroSkin.git .
  
  ## Update with pull
  git pull
  ```

### Fonts

This skin uses Segoe UI & Helvetica Neue (MacOS) by default.

Edit `custom.syles` to change this to something else, like:

- [Fira Sans source](https://github.com/mozilla/Fira) - [download](https://fonts.google.com/specimen/Fira+Sans)

- [Open Sans source](https://github.com/googlefonts/opensans) - [download](https://fonts.google.com/specimen/Open+Sans#standard-styles)

### License

- Metro for Steam [MIT License](https://choosealicense.com/licenses/mit/)

- Unofficial Patch [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa]. 
  [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg