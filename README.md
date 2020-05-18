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
12. Scan downloads with VirusTotal, but be aware of their privacy policy (use it to scan installers you've downloaded, but not personal documents, because people can use the VirusTotal API to see uploads)
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
36. Check firewall settings
37. Be aware that some malware tries to hide itself from you
38. Use 2FA
39. Monitor bank statements and account logins
40. Check out any entries in HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run in regedit
41. Scan websites with VirusTotal before going to them
42. Limit the number of Wordpress or other CMS sites you visit, considering that they are often targets for hacking, and could be used to deliver malware to users, even if the site owners themselves are legitimate
43. Only use remote access software if it's absolutely necessary
44. Be careful when doing port forwarding, and in general, it's best not to
45. Don't use UPnP
46. Check your network firewall with Gibson ShieldsUp
47. Check your computer's ports and services with nmap
48. Monitor traffic with Wireshark
49. Check your DNS settings with ipconfig /all, make sure it's not set to something suspicious
50. Monitor resource usage
51. Be aware that blue screens and other stability issues can sometimes be due to bad hardware or software, but sometimes also due to malware or security exploits
52. Some other "second opinion scanners" to use include Hitman Pro, Sophos, Bitdefender, etc.
53. Don't ignore SSL warnings in browsers
54. Run `Get-ScheduledTask` in PowerShell to see scheduled tasks
55. Check the Task Scheduler program (type in search bar)
56. Check WMI events by going to start -> run -> wmimgmt.msc, though they should also be displayed in AutoRuns
57. If you need to get files off of an infected computer, use a Linux flash drive, boot from that, and then use `ntfs-3g` to mount it, then get the files off. This can be more difficult if you are using BitLocker in Windows though.
58. If a malicious file is in your cloud storage (Dropbox, Google Drive, etc), then simply reinstalling your OS won't get rid of it, so you have to scan cloud storage as well
59. For SMB stuff/network-mapped drives, file versioning or offline/read-only backups are important to protect againt ransomware
60. Don't use Adobe Flash anymore
61. Make sure OS and program settings are set up correctly
62. If someone gets malware once, they not only have to get rid of it with anti-malware software, but they also need to change their habits to make sure they won't get it a second time.
63. Don't use old versions of Windows (XP, Vista, 7, etc)
64. Don't use Internet Explorer or Edge
65. Check your PATH variable
66. Keep track of what programs are installed, as they need to be updated, and you should keep up to date with CVEs that affect the programs you use
67. If you buy a used computer instead of a new one, either do a factory reset, or just buy a new copy of Windows, reformat the drive, and then reinstall the OS. There could be malware hidden on the computer that isn't obvious.
68. If you use something like PuTTY, make sure you download the legitimate one, not the numerous trojanized illegitimate versions of it
69. Make sure you have your UAC settings set to be relatively strict
70. Some cheap devices from Amazon or ebay (smart watches, expansion cards, etc) might come with software that is malicious, such as drivers, an app, etc. Be careful about the devices you use with your computer, as they might not be trustworthy.
71. If someone has physical access to your computer, it's not secure. So if you go to a library, get your laptop out, and then leave it unattended for a while, that's not safe.
72. Use a VPN, especially if you're on public wifi. But in general, public wifi is not safe to use.
73. Try to avoid sites that don't use HTTPS
74. Most of the time, computer security threats can be the result of clicking on something, like going to a website, opening an email attachment, installing a program, etc. However, sometimes there are security issues that don't require any user interaction at all, such as remote code execution issues. This is why it's important to update both your OS and the programs you have installed within it.
75. Be aware that some rootkits can persist even across factory resets or OS reinstallations, so doing stuff like reflashing your BIOS and reinstalling router firmware can be good.
76. Disable remote access on your router. Only allow it to be logged into from the local network.
77. Don't reuse passwords
78. Change your router's default admin password, and possibly the username as well, though not all firmware supports this.
79. It can be a good idea to use something liek pfSense, DD-WRT, or OpenWRT on a router, as many home router manufacturers won't give security updates for very long.
80. Sometimes, malware might have new files and new processes, but in other cases, malware might be changing Windows DLLs, so rather than being new files, they are merely modifications of legitimate things.
81. Foronics DeepFreeze can be a good way to make sure that malware can't stay on a system. It's mostly used by schools and businesses, but it could potentially be useful in a home environment too.
82. Don't disable your ad blocker, even if a website tells you to
83. Don't write passwords down in a text document. Only use a secure password manager, like LastPass (cloud-based) or KeePass (offline).
84. Don't use Avast antivirus. They sell your personal info. 
85. Look into Windows Sysinternals tools
86. Use Sysmon
87. If you get malware, change all your passwords
88. Don't think that switching to macOS or Linux will mean you no longer have to worry about security. Security is an issue for every single operating system.
89. Use Bitlocker, but just know that it can make file recovery more difficult if you need to use a bootable Linux flash drive for file recovery.
90. Not all security issues involve malware. For example, if you go to a website that has a cross-site scripting vulnerability, someone could write an XSS payload that will steal your cookies from that site. But that won't involve any malware on your computer. Endpoint security, network security, and account security are different things, but all very important.
