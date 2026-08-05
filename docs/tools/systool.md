# Stellar Data Recovery

Stellar Data Recovery is a data recovery software and services organization focused on recovering lost, deleted, formatted, corrupted, or inaccessible data from storage media and related systems. Stellar's current product portfolio includes data recovery software for Windows and macOS, recovery tools for specialized storage environments, and related file-repair and data-care products. [1][2]

## History

Stellar states that it has been developing data-care solutions since 1993. The company describes its activities as covering data recovery, data erasure, mailbox conversion, and file repair software and services. It operates from India and maintains offices in the United States and Europe. [1][3]

The company has developed its data-recovery portfolio for consumer, professional, and enterprise use cases. Its current recovery products cover Windows and macOS systems, as well as specialized recovery scenarios involving RAID, Linux storage, virtual-machine disks, and NAS devices. [2][4]

## Products

Stellar's product range is broader than disk recovery alone. The products below are the most relevant to data recovery and digital-forensics research.

### Stellar Data Recovery

Stellar Data Recovery is the company's general-purpose recovery product for Windows and macOS. It is intended to recover lost or deleted files from storage devices including hard drives, SSDs, USB drives, and memory cards. The Windows product documentation describes recovery scenarios including accidental deletion, formatting, partition loss, drive errors, and unbootable systems. [2][5]

### Stellar Data Recovery Professional

The Professional edition provides additional recovery capabilities for Windows and is also offered for macOS. Stellar describes it as supporting recovery from deleted, formatted, corrupted, encrypted, or inaccessible storage, including HDDs and SSDs. [6][7]

### Stellar Data Recovery Technician

The Technician edition is aimed at professional recovery work and includes RAID-oriented recovery capabilities. Stellar currently describes support for RAID 0, RAID 5, RAID 6, and hybrid RAID recovery scenarios. [2]

### Stellar Toolkit for Data Recovery

Stellar Toolkit for Data Recovery is intended for broader recovery scenarios involving Windows, macOS, and Linux storage. Stellar documents support for Windows file systems such as NTFS, FAT16, FAT32, and exFAT; macOS file systems including APFS, HFS, and HFS+; and Linux file systems including Ext2, Ext3, and Ext4. The toolkit also documents recovery from virtual-machine disk formats such as VMDK, VDI, VHD, and VHDX. [4]

### Stellar Photo Recovery

Stellar Photo Recovery is focused on recovery of photographs, videos, and audio files from storage media such as memory cards, flash drives, HDDs, and SSDs. [2]

### Related Stellar Products

Stellar also develops products for file repair, email recovery, mailbox conversion, database repair, data erasure, and other data-care tasks. These products should be distinguished from the general-purpose data-recovery products when documenting forensic workflows. [2]

## Data Recovery Capabilities

Depending on the product and operating system, Stellar documents recovery capabilities for scenarios including:

* Deleted-file recovery
* Lost-file recovery
* Formatted-volume recovery
* Lost or deleted partition recovery
* Recovery from corrupted or inaccessible volumes
* Recovery from RAW volumes
* Recovery from unbootable systems
* Recovery from HDDs and SSDs
* Recovery from USB flash drives and memory cards
* RAID recovery in supported editions
* Recovery from supported Linux and macOS file systems
* Recovery from supported virtual-machine disk images
* Recovery from selected NAS storage systems [4][5][6]

Recovery success is dependent on the condition of the source media, file-system state, overwriting, device behavior, and the recovery method used. SSD recovery can be particularly affected by mechanisms such as TRIM and subsequent data reuse.

## Supported Storage Media

Stellar documentation identifies a range of supported storage media and devices, including:

* Internal hard disk drives
* Solid-state drives (SSD)
* External hard drives
* USB flash drives
* SD and other memory cards
* Optical media in supported products
* RAID storage in supported editions
* Selected NAS devices
* Virtual-machine disk images in supported products [2][4][6]

Support varies by product, edition, operating system, and software version. Investigators should record the exact product and version used during an examination.

## File Systems

Documented file-system support varies between products. Current Stellar documentation identifies support for combinations of:

* NTFS
* FAT16
* FAT32
* exFAT
* ReFS
* APFS
* HFS
* HFS+
* Ext2
* Ext3
* Ext4 [4][6][7]

The presence of a file system in a product description does not by itself establish that every feature or recovery mode supports that file system. File-system and platform support should therefore be verified against the version used for an examination.

## File Types

Stellar Data Recovery documentation describes recovery of a broad range of file categories, including:

* Documents
* Images
* Video
* Audio
* Archives
* Email and mailbox data
* Databases
* Other user files supported by the selected recovery engine [6]

Specific extensions and supported formats vary by product and version.

## Forensic Relevance

Stellar Data Recovery is primarily marketed as data-recovery software rather than as a complete digital-forensics examination platform. It can nevertheless be relevant to forensic work when an examiner needs to locate or recover files that are deleted, lost, formatted, inaccessible, or otherwise difficult to access using normal operating-system tools.

Potential forensic uses include:

* Recovering deleted files from a forensic working copy
* Recovering files from damaged or inaccessible volumes
* Examining supported file systems for lost or deleted content
* Recovering data from supported RAID configurations
* Recovering files from supported virtual-disk images
* Identifying files that may require subsequent forensic examination

Use of a recovery utility should be treated as one examination step rather than as a substitute for forensic acquisition, preservation, analysis, and reporting.

## Evidence Handling Considerations

When Stellar software is used during a forensic examination, the examiner should preserve the original evidence and perform recovery from an appropriate forensic image, clone, or verified working copy whenever practical.

The following information should be documented:

* Evidence identifier
* Source device and media type
* Acquisition method
* Acquisition date and time
* Cryptographic hash values of the original and forensic image, where applicable
* Operating system used for the examination
* Stellar product name and exact version
* License or edition used, where relevant
* Scan type and recovery options
* File-system identified on the source
* Source image or working-copy identifier
* Destination used for recovered files
* Hash values of exported evidence, where applicable
* Any errors, warnings, or unusual recovery results

Stellar states on its product documentation that its Windows recovery software scans drives in read-only mode. This vendor statement should not be treated as a substitute for an examiner's own validation of the complete forensic workflow, because operating-system mounting, destination handling, imaging, and other examination activities can independently affect evidence or associated metadata. [6]

## Recovery from Disk Images

Stellar Toolkit for Data Recovery documents workflows for creating and scanning disk images and for recovering data from supported virtual-machine disk formats. For forensic use, an examiner should normally create and preserve a forensic acquisition independently and use a verified copy for recovery rather than relying on the recovery software itself as the primary acquisition mechanism. [4]

## RAID Recovery

Stellar Data Recovery Technician and Stellar Toolkit for Data Recovery document RAID-related recovery capabilities. Supported scenarios and RAID levels depend on the product and version. RAID reconstruction parameters should be recorded because incorrect parameters can produce incomplete, misleading, or corrupted recovery results. [2][4]

## Virtual Machine Recovery

Stellar Toolkit for Data Recovery documents support for virtual-machine disk formats including VMDK, VDI, VHD, and VHDX. These formats may contain complete operating-system volumes and should be handled as evidence containers when acquired during an investigation. [4]

## Operating Systems

Stellar provides recovery products for:

* Microsoft Windows
* macOS

Some Stellar recovery products can also recover data stored on Linux-formatted media while running from a supported Windows environment. The operating system of the examination workstation and the operating system represented by the evidence should be recorded separately. [4]

## Client Base

Stellar describes its products as serving consumer, professional, and enterprise data-care requirements. Its company information also identifies a global presence and states that its products and services are used across 190 countries. These figures are company-reported and may change over time. [1]

For forensic documentation, a distinction should be made between ordinary data-recovery customers and organizations using recovery software as part of an investigative or laboratory workflow.

## Significant Events

* **1993** — Stellar states that its data-care operations date to 1993. [1]
* **2025–2026** — Stellar continued to update its data-recovery products for newer operating systems, hardware, and storage environments. [8]
* **January 2026** — Stellar announced upgraded Windows and Mac data-recovery software, describing improvements including faster deep scans and support for newer operating-system and hardware environments. [8]
* **2026** — Stellar's published toolkit documentation identifies support for Windows, macOS, and Linux storage, virtual-machine disk formats, and selected NAS environments. [4]

## Limitations

The capabilities of Stellar products vary by product, edition, operating system, and version. The following limitations should be considered when evaluating results:

* Recovery is not guaranteed for overwritten data.
* SSD recovery can be affected by TRIM and other storage-controller behavior.
* Physical media failure may require specialist hardware-based recovery rather than software recovery.
* File-system support differs between products.
* RAID recovery depends on correct identification or reconstruction of the array configuration.
* Recovered files may not retain all original metadata or directory information in every recovery scenario.
* File-signature or RAW recovery may recover content without the original file-system context.
* A successful preview or recovery result does not by itself establish the authenticity or forensic significance of a recovered file.

## Versioning

Software behavior and supported platforms change between releases. A forensic report should identify the exact Stellar product, edition, version, operating system, and relevant configuration used during the examination.

Where possible, the examiner should retain the installer or other software-identification evidence required to reproduce or explain the examination.

## External Links

* [Official Stellar website](https://www.stellarinfo.com/)
* [Stellar Data Recovery for Windows](https://www.stellarinfo.com/windows-data-recovery.php)
* [Stellar Data Recovery for Mac](https://www.stellarinfo.com/data-recovery-mac.php)
* [Stellar Toolkit for Data Recovery](https://www.stellarinfo.com/data-recovery-toolkit.php)
* [Stellar download center](https://www.stellarinfo.com/download.php)
* [Stellar company overview](https://www.stellarinfo.com/company/about/stellar-overview.php)
* [Stellar support and documentation](https://www.stellarinfo.com/support/)

## References

1. Stellar, "Stellar Overview", company information.
2. Stellar, "Download Center", current product and edition listings.
3. Stellar, "Offices", company locations and global presence.
4. Stellar, "Data Recovery Toolkit", product capabilities and supported file systems, virtual-machine formats, and recovery workflows.
5. Stellar, "Windows Data Recovery", product capabilities and supported recovery scenarios.
6. Stellar, "Professional Data Recovery Software", product capabilities, supported media, file systems, and vendor-described read-only scanning.
7. Stellar, "Mac Data Recovery Software", supported Mac recovery scenarios and file systems.
8. Stellar, "Stellar Rolls Out Massive Upgrades to Data Recovery Software", 28 January 2026.
