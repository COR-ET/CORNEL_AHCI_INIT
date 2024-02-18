# CORNEL_AHCI_INIT
Load AHCI Devices and Storage (SATA) Devices in Kernel

# Usage :

** To load AHCI Devices and Init them: **
```cs
 AHCI_DISK ahci_load = new();

 ahci_load.Init();
```

** To Check if SATA Devices Initialized: **
```cs
AHCI_DISK.Check(); // Will print results and amount of SATA Devices
```

Then you can load your AHCI-SATA Storage Device :
```cs
var MainStorageBlockDevice = SATA.Devices[0];
Disk disk = new(MainStorageBlockDevice);
```

**Don't forget support ;)**
