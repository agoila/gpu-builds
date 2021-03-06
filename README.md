# gpu-builds
A non-exhaustive list of GPU builds to help those working on setting up their own on-prem DL solution.

## Fairly cheap builds
- [Single GTX 1080 ($850)](https://pcpartpicker.com/user/quietning/saved/#view=YP6v6h)
- [Single GTX 1080 ($1220)](https://pcpartpicker.com/list/qQhVBP)
- [Single GTX 1070 ($1185)](https://pcpartpicker.com/list/Df2KNN)


## Premium builds
- [Twin GTX 1080 ($2150)](https://pcpartpicker.com/user/maxdavis/saved/dvmkLk)
- [Twin GTX 1080 ($3250)](https://pcpartpicker.com/list/4zRqHN)


## Quad GPU build

Component | Link | Price | Comments
--- | --- | --- | ---
Motherboard | [ASUS EATX DDR4 LGA 2011-3 Motherboards X99-E](https://www.amazon.com/Asus-Motherboards-WS-USB-3-1/dp/B00XUDLXJG) | $509 | The key is that it is wide enough to support four double-width cards
CPU | [Intel Boxed Core i7-6850K Processor](https://www.amazon.com/gp/product/B01FJLAITC) | $425 | The key is that it has 40 PCI lanes so that all four cards can run at 8x PCI
RAM | [Corsair Vengeance LPX 64GB DDR4 2400](https://www.amazon.com/gp/product/B01ET6Y09C) | $720 | Any DDR4 2400 RAM is good
CPU Cooler | [Cooler Master Hyper 212 Evo Cooler](https://www.amazon.com/dp/B005O65JXI) | $30 | 
Hard Drive | 2x [Samsung 850 EVO 1TB 2.5-Inch SATA III Internal SSD](https://www.amazon.com/gp/product/B00OBRFFAS) | $350 | You can buy as many as you need. I'd recommend at least 2.
GPUS | 4x 1080 Ti (make sure to get "Founder's Edition" -- without any extra fans, which will mess up the case airflow) |  | 2 GPUs is also good.
Power Supply | [EVGA SuperNova 1600W](https://www.amazon.com/EVGA-SuperNOVA-PLATINUM-Crossfire-220-P2-1600-X1/dp/B00NJG61JQ) | $280 | If only using 2 GPUs, can go down to 1000W
Case | [Corsair Carbide Series Air 540 High Airflow ATX Cube Case](https://www.amazon.com/gp/product/B00D6GINF4) | $137 | Love this case -- enough room to comfortably fit everything.

### Tricks

SecureBoot must be disabled in the BIOS (which is done via the option to "Delete PK Keys").
If this isn't done, you will suffer from horrible installation troubles later on.

BIOS is accessible by pressing `Del` during bootup.

### Hard Drives

Two SSDs are RAID-0'd into a single Volume using the Intel Smart Storage thing, accessible by pressing `Ctrl+I` during bootup (see motherboard manual).

The remaining two SSDs serve as separate data drives.

