# Windows security

1. Install updates
2. Use a separate user and administrator account
3. Use Windows Defender and Malwarebytes Premium
4. Use a "second opinion scanner" if necessary
5. Check msconfig (specifically the "services" tab) and the task manager startup tab
6. Use Firefox and Chrome
7. Use uBlock Origin and HTTPS Everywhere in browsers
8. Back up your files to a FreeNAS server that uses ZFS snapshots (to protect against ransomware)
9. Make an Acronis image that you can revert back to if need be
10. Create restore points of known good configurations
11. Check Windows Event Viewer
12. Scan downloads with VirusTotal, but be aware of 
13. Use PowerShell to verify checksums
14. Use a VPN, preferably one that blocks known malicious domains
15. Use a DNS server that blocks malicious domains
16. Use Ninite Updater to keep non-OS things up to date
17. When running a Malwarebytes scan, check the "check for rootkits" box
18. Be careful about email attachments or clicking links
19. If you get malware, reformat your drive, reinstall Windows (or restore an Acronis image), and also reflash your BIOS
20. Keep your router firmware up to date and make sure it's secure, because an insecure network means an insecure computer
21. Check for things in C:\Users\current_user\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup\ 
22. In Explorer, check to view file extensions and hidden files
23. Be careful about installing programs
24. Only install or run programs with the minimum permissions required (as in, don't run everything with elevated privileges)
25. Be careful about opening word documents or PDFs, and don't enable word macros
26. If something crashes, that could possibly be a sign of an unstable exploit that does something like a buffer overflow or whatever
27. Check services.msc
28. Be aware that anti-malware software can have both false positives and false negatives
29. If you suspect something is wrong, then reboot into safe mode and then run your Malwarebytes scan (or whatever other scanner you use)
30. Use AdwCleaner if you suspect that you have adware
31. Use NoScript to disable JavaScript on web pages that you don't trust
32. Don't enable any sort of autoplay stuff for removable media
33. Use AutoRuns
34. Use Process Explorer
35. Check out BleepingComputer's tools
