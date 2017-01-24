# that-damn-backup

## Why
Single board computers (raspberry pi, odroid) are notorious for burning through their disk.
Since space/costs are limited, these devices use SD cards or eMMC memory for disk (in
addition to SoC ram). Flash memory is attrocious on write cycles and dies easily. This
project was born out of a frustration of handful of dead raspberry pis. Similarly, SSD or
USB controllers or SATA controllers can go bad. This will attempt to keep state on either
to a one week backup.

## What
Detects if computer has a mounted filesystem. If so, and large enough, back that data up.
Also works in reverse - if mounted FS is primary root, backup to the partition of the
flash memory.
