# nsp_update_patcher_mac
Fork of [willfaust's nsp_update_patcher script](https://gist.github.com/willfaust/fb90dec409b8918290012031f09a78ef) that is compatible with MacOS

### Important:
* Your free drive space should be at least **three times the size of your base and update NSPs combined**
* You **must** have your product keys dumped from **your Switch**

Credit to [hactool by SciresM](https://github.com/SciresM/hactool) and [hacPack by The-4n](https://github.com/The-4n/hacPack)

### Steps:
1. Install [Homebrew Package Manager](https://brew.sh/) if not already installed:
  ```bash
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```
2. Install depenencies:
  ```bash
  brew install gcc make grep curl
  ```
3. Create a new folder/directory and copy your base NSP, update NSP, and `prod.key` files to it
4. Open Terminal and enter folder/directory created in Step 3
5. Download scripts to folder/directory:
  ```bash
  curl -o nsp_update_patcher_mac.sh https://github.com/GumbyXGames/nsp_update_patcher_mac/blob/main/nsp_update_patcher_mac.sh
  ```
  ```bash
  curl -o nsp_update_patcher_mac_swapped.sh https://github.com/GumbyXGames/nsp_update_patcher_mac/blob/main/nsp_update_patcher_mac_swapped.sh
  ```
6. Make scripts executable:
  ```bash
  chmod +x nsp_update_patcher_mac.sh
  ```
  ```bash
  chmod +x nsp_update_patcher_mac_swapped.sh
  ```
7. Run script:

* If base NSP is bigger than udpate NSP:
    ```bash
    ./nsp_update_patcher_mac.sh
    ```
* If base NSP is smaller than update NSP: 
    ```bash
    nsp_update_patcher_mac_swapped.sh 
    ```
