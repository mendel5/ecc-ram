# ecc-ram

Everything you need to know about ECC RAM and how to use it in Windows and Linux

++ Work in Progress ++

## Links
### General
- https://en.wikipedia.org/wiki/ECC_memory
- https://www.memtest86.com/ecc.htm
- https://www.memtest86.com/compare.html
- https://forum.planet3dnow.de/index.php?threads/ecc-error-checking-correction-hauptspeicher-oder-ram.427046/
- https://blog.programster.org/how-to-check-for-ECC-ram-functionality
- https://www.phoronix.com/scan.php?page=news_item&px=Linus-Torvalds-ECC
- https://www.theregister.com/2021/01/04/linus_torvalds_intel_killed_ecc/
- https://www.realworldtech.com/forum/?threadid=198497&curpostid=198647 Linus Torvalds ECC Mailing list
- https://www.computerbase.de/2021-01/linus-torvalds-intel-ecc-standard/
- https://www.heise.de/hintergrund/Arbeitsspeicher-mit-Fehlerschutz-So-funktioniert-ECC-Speicher-6032966.html
- https://www.makeuseof.com/what-is-ecc-ram/
- https://www.pugetsystems.com/labs/articles/How-to-Check-ECC-RAM-Functionality-462/
- https://www.pugetsystems.com/labs/articles/Advantages-of-ECC-Memory-520/
- https://www.admin-magazine.com/HPC/Articles/Memory-Errors
- https://github.com/ThiagoMartinsdeMelo/Linux
- https://github.com/ThiagoMartinsdeMelo/Linux/blob/master/01%20-%20Hardware%20Information/checking%20ECC%20memory.md
- https://techlibrary.hpe.com/docs/iss/DL380pGen8/setup_install/advanced/Content/138605.htm Single bit vs multi bit ecc
- https://www.atpinc.com/blog/ecc-dimm-memory-ram-errors-types-chipkill Single bit vs multi bit ecc
- https://www.elektronik-kompendium.de/sites/com/1504141.htm
- https://www.tomshardware.com/news/intel-enables-ecc-on-12th-gen-core-cpus
- https://www.heise.de/news/Intel-Alder-Lake-Core-i-Prozessoren-mit-ECC-RAM-moeglich-6541388.html
- https://mcl.de/it-wissen/blog/rdimm-vs.-udimm-die-arbeitsspeicher-technologien-im-vergleich
- https://www.giga.de/extra/arbeitsspeicher/tipps/dimm-u-dimm-so-dimm-r-dimm-und-lr-dimm-was-ist-das-unterschiede-erklaert/
- https://linuxhint.com/rdimm-vs-udimm/
- https://www.computerbase.de/forum/threads/memtest-beim-asus-ws-c246-pro-wie-ecc-testen.2073239/ ECC Injection
- https://news.ycombinator.com/item?id=31016042 What Flips Your Bit: Cosmic Ray Errors at Mozilla (blog.mozilla.org)
- https://github.com/mchehab/rasdaemon
- https://www.setphaserstostun.org/posts/monitoring-ecc-memory-on-linux-with-rasdaemon/
- https://www.truenas.com/community/threads/ecc-working-single-multi-bit-testing-ecc-ram.72668/
- https://www.hardwareluxx.de/community/threads/fehlende-ecc-unterst%C3%BCtzung-linus-torvalds-schimpft-%C3%BCber-intel.1286407/page-2
- https://news.ycombinator.com/item?id=25622322 ECC matters (realworldtech.com) - Linus Torvalds
- https://lowendspirit.com/discussion/2369/linus-torvalds-hn-ecc-ram-rasdaemon

### Linux stuff
- https://www.admin-magazin.de/Das-Heft/2013/12/Speicherfehler-unter-Linux-erkennen-und-beobachten
- https://forum.ubuntuusers.de/topic/herausfinden-ob-ecc-aktiv-ist/

### Windows stuff
- https://docs.microsoft.com/en-us/windows/win32/cimwin32prov/win32-physicalmemoryarray
- https://answers.microsoft.com/en-us/windows/forum/all/enable-windows-10-pro-ecc-settings-whea-windows/221e6baa-a765-4cfb-800b-3b32fd6e9434
- https://www.der-windows-papst.de/2018/02/19/ecc-funktion-unter-windows-testen/
- https://forum.level1techs.com/t/how-to-validate-ecc-memory/140341

### Stack Exchange
- https://superuser.com/questions/893560/how-do-i-tell-if-my-memory-is-ecc-or-non-ecc
- https://superuser.com/questions/1635090/what-happened-to-ecc-ram
- https://superuser.com/questions/tagged/ecc?tab=Votes
- https://serverfault.com/questions/643542/how-do-i-get-notified-of-ecc-errors-in-linux
- https://unix.stackexchange.com/questions/139319/how-to-tell-whether-ram-ecc-is-working
- https://serverfault.com/questions/289098/what-is-the-difference-between-rdimm-vs-udimm

### Reddit
- https://www.reddit.com/r/HomeServer/comments/gh7r7q/how_to_log_corrected_ecc_memory_errors_in_windows/
- https://www.reddit.com/r/unRAID/comments/mc5d2h/understanding_the_realworld_effects_of_ecc_ram_in/
- https://www.reddit.com/r/Amd/comments/lerxuj/linus_was_right_consumer_ecc_memory/
- https://www.reddit.com/r/freenas/comments/o9sg8q/confused_about_ecc_memory_homelab/
- https://www.reddit.com/r/Amd/comments/np5m9m/use_of_ecc_ram/
- https://www.reddit.com/r/Amd/comments/lf3i6b/overclocked_ecc_memory_with_a_5900x_my_results/
- https://www.reddit.com/r/hardware/comments/t9jn2s/intel_enables_ecc_memory_on_consumer_alder_lake/
- https://www.reddit.com/r/Amd/comments/bsszwg/ecc_ryzen_and_2bit_errors/
- https://www.reddit.com/r/hardware/comments/mc8j2c/what_is_the_difference_between_ddr5_ecc_and_real/

### Youtube
- https://www.youtube.com/watch?v=pPeCNrNTr3k Linus was right, ECC Memory Explained by Linus Tech Tips
- https://www.youtube.com/watch?v=uTuxqxSkjYY Check for ECC memory using Windows 10 PowerShell commands
- https://www.youtube.com/watch?v=fCQYBsuBqfU Speicherdiagnose (RAM) mit Windows-Bordmitteln untersuchen: Arbeitsspeicher auf Fehler pr??fen

### New
- https://linustechtips.com/topic/952498-checking-ecc-error-count/
- https://www.reddit.com/r/HomeServer/comments/gh7r7q/how_to_log_corrected_ecc_memory_errors_in_windows/
- https://www.reddit.com/r/Amd/comments/ggmyyg/an_overview_of_ecc_memory_on_ryzen/
- http://www.xtremesystems.org/forums/showthread.php?283454-ECC-soft-error-count-reporting-monitoring-on-Windows
- https://answers.microsoft.com/en-us/windows/forum/windows_7-hardware/ecc-error-logging-and-reporting-in-windows-7/08c242c4-69ec-47c9-bf7c-0fe9c023e32f
- https://techreport.com/forums/viewtopic.php?t=81239

## Commands
### Linux
```
sudo dmidecode -t memory

sudo dmidecode -t 16
```

```
rasdaemon
```

### Windows
#### 1
In Windows CMD or Windows Powershell, enter the following command:
```
wmic memorychip get datawidth,totalwidth
```

Output:
```
# If the system has ECC memory
DataWidth  TotalWidth
64         72

# If the system does not have ECC memory
DataWidth  TotalWidth
64         64
```

#### 2
In Windows CMD or Windows Powershell, enter the following command:
```
wmic memphysical get memoryerrorcorrection
```

Output:
```
0 (0x0) Reserved 

1 (0x1) Other 

2 (0x2) Unknown 

3 (0x3) None 

4 (0x4) Parity 

5 (0x5) Single-bit ECC 

6 (0x6) Multi-bit ECC 

7 (0x7) CRC
```

Explanation:
- 0 Reserved:
- 1 Other:
- 2 Unknown:
- 3 None: The currently installed RAM modules do not support ECC.
- 4 Parity:
- 5 Single-bit ECC: Single bit errors are detected and corrected. Multi-bit errors are not detected and not corrected. (to verify!)
- 6 Multi-bit ECC: Single bit errors are detected and corrected. Multi-bit errors are detected and reported, but not corrected. (to verify!)
- 7 CRC: CRC stands for Cyclic redundancy check

## Todo
- Single bit ECC vs Multi bit ECC
- How to check if ECC Ram works in Synology Diskstation NAS?
- Terminal Commands for Windows 10, Linux and Synology
- R-DIMM/RDIMM, U-DIMM/UDIMM, SO-DIMM/SODIMM
- Registered / Unregistered, wohl identisch zu RDIMM, https://en.wikipedia.org/wiki/Registered_memory
- Buffered / Unbuffered, betrifft wohl nur RDIMM
- Synchronous / Asynchronous
  - https://en.wikipedia.org/wiki/Synchronous_dynamic_random-access_memory
- Compare:
  - https://geizhals.de/?cat=ramddr3
  - https://geizhals.de/g-skill-aegis-dimm-kit-16gb-f4-3200c16d-16gis-a2151626.html?hloc=de
  - https://geizhals.de/corsair-vengeance-rgb-pro-schwarz-dimm-kit-16gb-cmw16gx4m2c3200c16-a1828434.html?hloc=de
  - https://geizhals.de/kingston-server-premier-dimm-32gb-ksm32ed8-32me-a2351239.html?hloc=de
- ECC injection
- Rank: Single-Rank, Dual-Rank, Quad-Rank
  - https://techlibrary.hpe.com/docs/iss/DL380pGen8/setup_install/advanced/Content/138678.htm
  - More Ranks is better. Dual-Rank usually works very well.
- How about bandwidth? There's no excuse for not buying some Dual Rank B-die these days. My 3600c16 rated kit can do this and I'm motherboard limited. https://wccftech.com/nvidia-ad102-gpus-powering-next-gen-geforce-rtx-40-series-will-stick-with-pcie-gen-4-0-protocol/#comment-5837613568
- Single Channel vs Dual Channel (`2 x 4GB` is better than `1 x 8GB`) https://old.reddit.com/r/pcmasterrace/comments/ube2ze/me_right_now/
- AM4 doesn't support ECC RDIMMs on any level, it only supports normal (non-ECC) UDIMMs and ECC UDIMMs https://old.reddit.com/r/HomeServer/comments/duj1pf/am4_with_registered_ecc_ram/f76mdtg/
- Memtest86 vs Memtest86+: Memtest86 is a proprietary software sold by PassMark. Memtest86+ is FOSS. Memtest86 is preferred over Memtest86+ because Memtest86 has been optimized for UEFI, etc. https://en.wikipedia.org/wiki/Memtest86
- DDR5 On-die ECC vs. "normal" side-band ECC
