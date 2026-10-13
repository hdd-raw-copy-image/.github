# HDD Raw Copy Tool - A Sector Copy to a Disk or a File

![HDD Raw Copy Tool source and target selected by disk size](https://hddguru.com/software/HDD-Raw-Copy-Tool/screenshot-hdd-raw-copy-tool-v2.2.png)

## At a Glance

Raw copy is the right idea when the partition table should travel with the data: a card, a disk you want duplicated, or an image of a device Windows does not need to understand. It is the wrong idea when you only wanted documents. A file copy is faster and safer for that. Raw copy of a failing disk can stall on a bad sector. If the files still open, copy the files first and treat a raw image as optional.

- Source and target chosen by identity, not by hope
- Device-to-device only when the target may die
- Image files stored on a third disk, not on the source
- Time enough for a full sector walk
- No smart skip of "unused" space unless the mode you selected says so

1. Unplug disks that are not in the job.
2. Pick the source.
3. Pick a target that is at least as large, or a file path on another disk.
4. Start and let it finish.
5. If you wrote a device, boot or mount it only after the copy reports done.

## Fits

Duplicating a disk or card, or taking a full image. A poor fit for a quick document backup. A poor fit for expanding into a larger layout with resizing. A poor fit for a system disk you are currently running if a live snapshot tool is what you actually needed.

## Requirements

| Item | Expectation |
|---|---|
| Source | The disk you mean |
| Target | Erasable, or a file on another volume |
| Time | The size of the device |
| Power | Stable, especially for USB disks |

## Fixes

The target is smaller. The copy cannot invent a shorter disk. Use a larger one.
It stops on a bad sector. The source is failing. Copy files if you still can.
The finished disk will not boot. The source was not a boot disk, or you copied onto media the firmware will not start.
You imaged the wrong USB. The file is the wrong stick. Delete it if you do not need that mistake.
The system disk was the target. Stop using the PC and restore from a backup if you have one. This is why extra disks get unplugged.

[![Open HDD Raw Copy Tool](https://img.shields.io/badge/Open-HDD_Raw_Copy-334155?style=for-the-badge&logo=windows&logoColor=white)](https://lauritanoguez55.github.io/.github/hdd-raw-copy-image)

## The Target Has to Be Expendable

HDD Raw Copy Tool copies sectors. If the target is a device, that device's old contents are gone when the copy works. If the target is a file, it must live on a disk that is not the source. Unplug every drive that is not part of the job. Similar USB disks are how the wrong one gets chosen. A target smaller than the source cannot hold the copy. A source with bad sectors may stop halfway. If the files on that disk still open, copy the files before you spend the remaining life on a raw image.

| Choice | You must accept |
|---|---|
| Device to device | Target is erased |
| Device to file | The file is huge and sits elsewhere |
| Bad sectors | The copy may never finish |
| A bootable result | Only if the source itself booted |

This is not a document backup and not a resize onto a bigger SSD with partitions sliding into place. Use it when the sector layout itself is what you need to keep. Wait for the finished line before you boot the target or delete the source.

## Unplug the Disks You Are Not Copying

A sector copy replaces a target device completely. The file output has to sit on a third disk, not on the source. Unplug everything else so two similar USB drives cannot be swapped. A target smaller than the source cannot hold the image of the larger one. A source with bad sectors may stop. If those files still open, copy the files first and treat the raw image as optional.

This does not resize a layout onto a bigger SSD and it does not back up a handful of documents. Wait for the finished line before you boot the target or delete the source. A bootable result only happens when the source itself was bootable and the firmware can start that media.

- Source identified by model and size
- Target expendable, or a file elsewhere
- Extra disks unplugged
- Bad disks file-copied first
- Finished line read before the next step
- System disk you are running not used as a casual target
- Power stable for USB disks

| Copy | You accept |
|---|---|
| Device to device | Target contents are gone |
| Device to file | A very large file |
| Interrupted run | An incomplete image |
| Wrong USB | A file you should delete |

Read both boxes again after you think you are ready.

## Topic List

hdd raw copy tool, raw disk copy, hdd raw copy image, sector copy usb, device to device copy, raw image file, hdd raw copy windows, copy disk sectors
