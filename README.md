# Hackintosh EFI para MSI MAG B760M MORTAR WIFI DDR4

Este repositorio contiene la configuración EFI para ejecutar macOS Sequoia en mi configuración de hardware específica.

## Especificaciones de Hardware

- **CPU**: Intel Core i7-14700F @ 2.11 GHz (8 cores, 16 threads con Hyper-Threading)
- **Watercooling Cpu Id-cooling Frostflow 120x Intel Amd Oc**
- **Placa Base**: Mother Gigabyte Z790 AORUS ELITE AX WIFI DDR4 S1700 (supuesta basada en configuración típica)
- **Red**: Intel WiFi (usando itlwm) + Realtek Ethernet (RTL8125)
- **Bluetooth**: Intel Bluetooth (usando IntelBluetoothFirmware)
- **SMBIOS**: iMacPro1,1
- **RAM**: 32 GB
- **Almacenamiento**: [1 X Disco Solido SSD M.2 SK Hynix 2TB Platinum P41 7000MB/s NVMe PCIe Gen4 x4 Principal  , SSD 500GB, SSD 250GB]
- **Periféricos conectados**:
  - Teclado: Redragon (usando controlador SONiX)
  - Receptor Logitech USB
  - Controlador inalámbrico Sony
- **RX6600 XT 8GB**


## Versión de macOS

- macOS Sequoia 14.x.x

## Qué funciona

- ✅ CPU Power Management (con CpuTopologyRebuild)
- ✅ Gráficos (con WhateverGreen)
- ✅ Audio (con AppleALC)
- ✅ Ethernet (con LucyRTL8125Ethernet)
- ✅ WiFi (con itlwm)
- ✅ Bluetooth (con IntelBluetoothFirmware y BlueToolFixup)
- ✅ Monitorización del hardware (con SMCProcessor y SMCSuperIO)
- ✅ USB (todos los puertos)
- ✅ Sleep/Wake
- ✅ Servicios de Apple (iCloud, iMessage, FaceTime)

## Qué no funciona o tiene problemas

- [❌] [Completar según corresponda]
- [⚠️] [Funciones con problemas o limitaciones]

## OpenCore

- Versión: [Completar con la versión exacta]
- Configuración: [RELEASE/DEBUG]

## Kexts incluidos

- **Lilu.kext** (1.7.1) - Framework esencial para muchos otros kexts
- **VirtualSMC.kext** (1.3.6) - Emulación de SMC para sistemas no-Apple
- **SMCProcessor.kext** (1.3.6) - Monitoreo de CPU para VirtualSMC
- **SMCSuperIO.kext** (1.3.6) - Monitoreo de hardware para VirtualSMC
- **AppleALC.kext** (1.9.5) - Soporte para audio nativo
- **WhateverGreen.kext** (1.7.0) - Parches gráficos y mejoras
- **NVMeFix.kext** (1.1.3) - Mejoras para unidades NVMe
- **RestrictEvents.kext** (1.1.6) - Manejo de eventos del sistema
- **CpuTopologyRebuild.kext** (2.0.2) - Corrección de topología CPU
- **LucyRTL8125Ethernet.kext** (1.2.2) - Soporte para Ethernet Realtek 2.5G
- **itlwm.kext** (2.3.0) - Soporte para WiFi Intel
- **IntelBluetoothFirmware.kext** (2.5.0) - Soporte para Bluetooth Intel
- **BlueToolFixup.kext** (2.7.0) - Correcciones para Bluetooth
- **IntelBTPatcher.kext** (2.5.0) - Parches adicionales para Bluetooth Intel

## Notas importantes

- Esta EFI está configurada específicamente para una placa MSI MAG B760M MORTAR WIFI DDR4 con un procesador Intel Core i7-14700F.
- La configuración de SMBIOS está basada en iMacPro1,1.
- Siempre haz una copia de seguridad de tu EFI funcional antes de realizar cambios.
- Esta configuración fue creada siguiendo la [Guía de OpenCore](https://dortania.github.io/OpenCore-Install-Guide/).

## SMBIOS

- Modelo: iMacPro1,1




## Actualizaciones

- **[18/03/2025]**: Configuración inicial para macOS Sequoia.

## Contacto

- Para problemas relacionados con esta configuración específica, abre un issue en este repositorio.
