# ecc-ram

++Work in Progress++

Everything you need to know about ECC RAM and how to use it in Windows and Linux

## Links
- https://en.wikipedia.org/wiki/ECC_memory
- https://superuser.com/questions/893560/how-do-i-tell-if-my-memory-is-ecc-or-non-ecc
- https://superuser.com/questions/1635090/what-happened-to-ecc-ram
- https://superuser.com/questions/tagged/ecc?tab=Votes
- https://serverfault.com/questions/643542/how-do-i-get-notified-of-ecc-errors-in-linux
- https://unix.stackexchange.com/questions/139319/how-to-tell-whether-ram-ecc-is-working
- https://www.memtest86.com/ecc.htm
- https://docs.microsoft.com/en-us/windows/win32/cimwin32prov/win32-physicalmemoryarray
- https://answers.microsoft.com/en-us/windows/forum/all/enable-windows-10-pro-ecc-settings-whea-windows/221e6baa-a765-4cfb-800b-3b32fd6e9434
- https://www.der-windows-papst.de/2018/02/19/ecc-funktion-unter-windows-testen/
- https://forum.planet3dnow.de/index.php?threads/ecc-error-checking-correction-hauptspeicher-oder-ram.427046/
- https://forum.level1techs.com/t/how-to-validate-ecc-memory/140341
- https://www.admin-magazin.de/Das-Heft/2013/12/Speicherfehler-unter-Linux-erkennen-und-beobachten
- https://blog.programster.org/how-to-check-for-ECC-ram-functionality
- https://forum.ubuntuusers.de/topic/herausfinden-ob-ecc-aktiv-ist/
- https://www.reddit.com/r/HomeServer/comments/gh7r7q/how_to_log_corrected_ecc_memory_errors_in_windows/
- https://www.reddit.com/r/unRAID/comments/mc5d2h/understanding_the_realworld_effects_of_ecc_ram_in/
- https://www.reddit.com/r/Amd/comments/lerxuj/linus_was_right_consumer_ecc_memory/
- https://www.reddit.com/r/freenas/comments/o9sg8q/confused_about_ecc_memory_homelab/
- https://www.reddit.com/r/Amd/comments/np5m9m/use_of_ecc_ram/
- https://www.reddit.com/r/Amd/comments/lf3i6b/overclocked_ecc_memory_with_a_5900x_my_results/
- https://www.youtube.com/watch?v=pPeCNrNTr3k Linus was right, ECC Memory Explained by Linus Tech Tips
- https://www.youtube.com/watch?v=uTuxqxSkjYY Check for ECC memory using Windows 10 PowerShell commands
- https://www.phoronix.com/scan.php?page=news_item&px=Linus-Torvalds-ECC
- https://www.theregister.com/2021/01/04/linus_torvalds_intel_killed_ecc/
- https://www.realworldtech.com/forum/?threadid=198497&curpostid=198647
- https://www.computerbase.de/2021-01/linus-torvalds-intel-ecc-standard/
- https://www.heise.de/hintergrund/Arbeitsspeicher-mit-Fehlerschutz-So-funktioniert-ECC-Speicher-6032966.html
- https://www.makeuseof.com/what-is-ecc-ram/
- https://www.pugetsystems.com/labs/articles/How-to-Check-ECC-RAM-Functionality-462/
- https://www.admin-magazine.com/HPC/Articles/Memory-Errors
- https://github.com/ThiagoMartinsdeMelo/Linux
- https://github.com/ThiagoMartinsdeMelo/Linux/blob/master/01%20-%20Hardware%20Information/checking%20ECC%20memory.md

## Commands
### Windows
#### 1
```
wmic memorychip get datawidth,totalwidth
```
```
# Output:
# ECC Memory
DataWidth  TotalWidth
64         72

# Non-ECC Memory
DataWidth  TotalWidth
64         64
```

#### 2
```
wmic memphysical get memoryerrorcorrection
```

```
# Output:
0 (0x0) Reserved 

1 (0x1) Other 

2 (0x2) Unknown 

3 (0x3) None 

4 (0x4) Parity 

5 (0x5) Single-bit ECC 

6 (0x6) Multi-bit ECC 

7 (0x7) CRC
```
- 0 Reserved:
- 1 Other:
- 2 Unknown:
- 3 None: The currently installed RAM modules do not support ECC.
- 4 Parity:
- 5 Single-bit ECC:
- 6 Multi-bit ECC:
- 7 CRC: 

## Todo
- Single bit ECC vs Multi bit ECC
- How to check if ECC Ram works in Synology Diskstation NAS?
- Terminal Commands for Windows 10, Linux and Synology
