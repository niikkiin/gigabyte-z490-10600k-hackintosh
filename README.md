# My Personal OpenCore EFI for Gigabyte z490 10600k Hackintosh

![image](https://user-images.githubusercontent.com/26428605/172044995-39fca5e9-a2ab-4eb7-902f-d49edc064ece.png)

## Hardware specs

- Intel Core i7 10600k
- Gigabyte Z490 Aorus Elite
- TODO: add other specs

## What works

- CPU virtualization with Docker
- Front & rear USB ports
- Bluetooth

## Cloning

```shell
git init
git remote add origin git@github.com:niikkiin/gigabyte-z490-10600k-hackintosh.git .
git pull --set-upstream origin master
git submodule update --init --recursive
```

## Install

Just type `make install` to download OpenCore and ACPI/drivers/kexts for configured version.

## Cleanup

Type `make clean` to clean up any downloaded files to make your EFI folder structure look clean.

## Bootable USB Installer (WIP)

If you're installing EFI for USB Installer, you'll want to display console messages during boot for troubleshooting. I've made a special target that can run after install to enable verbose mode in `config.plist`, just run: `make install_usb`.

## Disclaimer

This OC build is made specifically for my system. Don't use it unless you understand which configurations need to be changed to suit your need. Checkout [merged PRs](https://github.com/niikkiin/gigabyte-z490-10600k-hackintosh/pulls) for some important changes.

## Credits

- [acidanthera](https://github.com/acidanthera)
- [Dortania's OpenCore Install Guide](https://dortania-github-io.thrrip.space/OpenCore-Install-Guide/)
- [tuanht/hackintosh-10600k-z490-aorus-elite-5700xt](https://github.com/tuanht/hackintosh-10600k-z490-aorus-elite-5700xt/blob/master/README.md)

