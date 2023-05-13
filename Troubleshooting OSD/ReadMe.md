### Find missing drivers in WinPE
Enable troubleshooting cmd F8. <br>

### To query WMI
Use wbemtest.

### Check if network card loaded 
wmic nic get netconnectionid

### Find Network card 
Select * from Win32_PNPEntity where description LIKE '%ether%' <br>
Select * from Win32_PNPEntity where description LIKE '%Network%'

### To inject driver from cmd
Download appropriate driver from Windows Update Catalog or vendor site. <br>
Extract the files. <br>
Load them using "drvload filepath"

### Initialize network card
wpeutil initializenetwork

### Restart task sequence
tsbootshell
