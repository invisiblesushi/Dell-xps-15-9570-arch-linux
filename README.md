# Dell XPS 15 9570 Arch linux configuration

### BIOS / UEFI
* Disable secure boot
* SATA to AHCI

### Kernel parameters
* `GRUB_CMDLINE_LINUX_DEFAULT="quiet pcie_aspm=force acpi_osi=Linux mem_sleep_default=deep acpi_rev_override=1 scsi_mod.use_blk_mq=1 drm.vblankoffdelay=1 >`

### Undervolt
Intel 8750h

/etc/intel-undervolt.conf
```
undervolt 0 'CPU' -150
undervolt 1 'GPU' -25
undervolt 2 'CPU Cache' 0
undervolt 3 'System Agent' 0
undervolt 4 'Analog I/O' 0
```
