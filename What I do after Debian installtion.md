# Howdy in Debian
 Howdy provides Windows Hello™ style authentication for Linux. Use your built-in IR emitters and camera in combination with facial recognition to prove who you are.
    
## Installation
- Step 1:
    ```
    sudo apt update
    ```     
 - Step 2:
  Download the .deb file from the [Releases page](https://github.com/boltgolt/howdy/releases).
  Latest version 2.6.1

- Step 3:
    ```sh
    cd Downloads
    sudo apt install ./howdy_2.6.1.deb -y
- Step 4:
  To avoid the Camera path error, Manually check path of webcam. [#281](https://github.com/boltgolt/howdy/issues/281)
  `sudo howdy config` then find the value `device_path` adding `/dev/videoX` after euqal symbol (x will be numbers Try running `ls /dev | grep video` to determine webcam name)
  
## Setup
- Step 1
After installation, Howdy needs needs to learn what you look like so it can recognise you later. Run `sudo howdy add` to add a face model.
After installation, Howdy needs to learn what you look like so it can recognise you later. Run `sudo howdy add` to add a face model.
If nothing went wrong we should be able to run sudo by just showing your face. Open a new terminal and run `sudo -i` to see it in action. Please check [this wiki page](https://github.com/boltgolt/howdy/wiki/Common-issues) if you've experiencing problems or [search](https://github.com/boltgolt/howdy/issues) for similar issues.

## Final
try to lock screen to see if howdy works correctly. enjoy.