# k3s-pi-cluster
Documenting my journey into kube pi clustering

## Equipment
- 2x 128GB Sandisk Extreme microSD cards - https://www.costco.com/sandisk-extreme-plus-128gb-microsd-card-with-adapter%2C-2-pack.product.100485627.html
- 2x Rasberry Pi 4 8GB boards - https://makerbright.com/raspberry-pi-4-8gb.html
- 2x Rasberry Pi 4 power supplys - https://makerbright.com/official-raspberry-pi-4-psu.html
- 2x Board heatsink/coolers - https://smile.amazon.com/gp/product/B07VWM4J4L/ref=ppx_yo_dt_b_asin_title_o03_s00?ie=UTF8&psc=1
- Wireless Keyboard/Trackpad - https://smile.amazon.com/gp/product/B014EUQOGK/ref=ppx_yo_dt_b_asin_title_o03_s00?ie=UTF8&psc=1
- Rack mount kit - https://www.uctronics.com/uctronics-for-raspberry-pi-rack-with-micro-hdmi-adapter-boards-19-1u-rack-mount-supports-1-4-units-of-raspberry-pi-4-model-b-u6128.html


## Stetup
1 - Install Rasbian lite on SD cards
  - Download Rasberry Imaging tool - https://www.raspberrypi.org/software/
  - Load latest version of Rasbiean Lite onto SD cards (2021-01-11 at time of writing)
2 - Change password from default (security is important)
3 - Enable SSH
  - Several ways to do this, but I happen to have setup easy console access.
    - Login via console
    - `sudo raspi-config`
    - Select `Interfacing Options`
    - Select `SSH` and enable it
    - Exit
4 - Upgrade to latest version of Rasbian becuase you put off doing this for over 6 months :D.
  - `sudo apt update`
  - `sudo apt full-upgrade`
  - `sudo reboot`
