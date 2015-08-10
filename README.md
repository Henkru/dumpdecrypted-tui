This is simple text-based user interface with [dumpdecrypted].

Usage:

```
iPhone:~ root# ./dumpdecrypted-tui
Select the encrypted App
1) MobileMail.app	           7) DDActionsService.app
2) WebContentAnalysisUI.app    8) MobileSafari.app
3) Calculator.app	           9) Scan.app
4) WebViewService.app	      10) Web.app
5) StoreKitUIService.app
6) Weather.app
#? 9
mach-o decryption dumper

DISCLAIMER: This tool is only meant for security research purposes, not for application crackers.

[+] Found encrypted data at address 00002000 of length 1826816 bytes - type 1.
[+] Opening /private/var/mobile/Applications/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/Scan.app/Scan for reading.
[+] Reading header
[+] Detecting header type
[+] Executable is a FAT image - searching for right architecture
[+] Correct arch is at offset 2408224 in the file
[+] Opening Scan.decrypted for writing.
[-] Failed opening. Most probably a sandbox issue. Trying something different.
[+] Opening /private/var/mobile/Applications/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/tmp/Scan.decrypted for writing.
[+] Copying the not encrypted start of the file
[+] Dumping the decrypted data into the file
[+] Copying the not encrypted remainder of the file
[+] Closing original file
[+] Closing dump file
```

[dumpdecrypted]:https://github.com/stefanesser/dumpdecrypted
