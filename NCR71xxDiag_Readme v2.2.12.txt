NCR71xxDiag
Readme File
Version: 2.2.12
Copyright © 2020. NCR Corporation.
All rights reserved.
________________________________________________________________________________


This file provides information on how to install the NCR71xxDiag.

Download and run the NCR71xxDiag Utility Install.exe file. 

The installation will install the NCR71xxDiagInstall.exe in the following directory by default:

C:\Program Files\NCR\Retail Utilities

It will create a shortcut on the desktop to the executable.

It will also create a shortcut to the executable under "C:\Program Files\NCR\Retail Utilities"


Windows Installer Merge modules for required system files are executed and these 
Required system files are installed if they do not already exist on the terminal.

These are for the files:

MSCOMCTL.OCX
MSWINSCK.OCX

Revision History:
Version 2.2.12 Release:
New Feature added
1. Min rec length - all the options added includeing 4 inch.
2.EEPROM Reset default added.
Known Issues:
1.After pressing "EEPPROM default" followed by "Restart" button printer gets Disconnected automatically in NHPI mode.
2.After pressing "EEPROM default" button ,followed by "Restart" and "print dianostics" .printing gets stop in middle ,printer going in error mode.

Revision History:
Version 2.2.11 Release:

New Features are added:
1.Added 7199 Printer as Printer Model.
-Features added for 7199 Printer:

	a.Communication Interface:
		i.Added USB Speed
	b.Change Configuration:
		i.Added 'Compatible Top Margine' to the Emulation/Software.
		iii.'Buzzer Tone' is added to the Hardware.
	c.View Tally:
		 i.Added the seperate condition for 7199 Printer to Apply&Print option.
 		ii.Added seperate condition of 'WaitForSingleObject' with different parameters. (4000 miliseconds)
		iii.Added the condition to print the text on Receipt when Apply&Print will be select. 

2.POS Printer Type: Model list is updated.
3.NCR HID Printer Interface: Updated Product ID list, if user select Port Number as NHPI and Model as any printer (ex:7199) then Product ID list should contain only "Any HID USB POS Printer" & selected printer (NCR 7199). 

Fixed Issues:
1.Runtime Error after change the Color Paper to Two color, restart the Printer & click on Two Color button.	
2.Printer status going to Offline mode after select and change of the multiple tallies from Printer Tally.
 


Revision History:
Version 2.2.10 Release:
New Features are added
1. NCR71xxDiag.exe needs to report error if wrong baud rate, data, stop, or parity are set.
2. Export to File: All the configuration, which user has selected can be saved in a file.
3. Import to File: All the user saved configurations will be selected automatically, when user import that file.
4. Added NHPI Interface support.
Fixed Issues:
1. Added 1256 Code Page for Series II printers.
2. Run Time Mismatch Error after printer restart.
3. No Value observed in "Receipt Lines (Back)" Tallies in 7198 2ST Printer.
4. Connect button still enabled after successfully connecting to printer.
7. Not able to connect to printer after changing the communication interface to NHPI
8. 7197 R2 printer goes offline on "Restart Printer(2)" operation.
9. "Printer is not connected. Verify the communication parameters" error observed although printer was configured and connected properly.
10. Printer options are not enabled after printer restart.
11. RunTime error occurred while importing the file for hardware options.
12. Run time error occurred while importing the  code page option file.
13. "Apply to Printer" is behaving same as "Apply and Print" operation.
14. 48 Char print option is not enabled while switching between dialogs, after printer restart.
15. Disabled settings are enabled when restarting the printer manually.
16. New imported file cannot overwrite previous imported file settings.
Known Issues:
1. Crash when performing SLIP operation in 7167 using NHPI connection 
2. Crash when printing "Two Side Print (4)" using NHPI connection
3. Crash after printing receipt in SSCO 6 Printer using NHPI connection.
The above known issues are under investigation and the fixes will be available in the next release.

Revision History:
Version 2.2.9 Release:
1) Changed the parameters for 7168 and 7167/7197 series II printers “Max Power” option in Hardware   configuration 
7167SII & 7197SII power modes:
        1. Term Pwr-High
	2. NCR 75W Ext Pwr
	3. Term Pwr-Low
	4. NCR 60W Ext Pwr
7168SII power modes:
	1. NCR Term Pwr
	2. NCR 75W Ext Pwr
2) Fixed the GUI Issues

Revision History:
Version 2.2.8 Release:
1) Fixed file already open issue
2) Changed the Change configuration buttons alignment and ordered the clipped string
3) Disabled the slip option in tally window for kiosk printer

Version 2.2.7 Release:
Fixed Issues:
1) The printer parameters will not reset after applying the settings to the printer.
2) After restarting the printer, printer should connect automatically. No need of going back to main window again
3) When switching between dialogs of Hardware / Emulation / Communications/ etc. when you select and option any previously chosen options need to be shown.
4) Added CLEAR and CLEARALL options to set the options
5) Added APPLY ALL OPTIONS that will write all selections from all dialogs out to the printer.
6) CREATE BINARY SETTINGS FILE and CREATE BINARY SETTINGS FILE WITH RESET when Apply or Apply ALL button is clicked
7) Changed to Part Number under Boot Firmware on View Tally (V) to read-only


Fixed Issues:
1. Able to communicate with printer using serial communication with all the parity parameters (None/Even/Odd)

2. Added the Xon/Xoff hand shaking requirement

3. Added the support SSCO 6 Printer 

Version 2.2.3 Release:


Fixed Issues:

1. Check Scan operation error has been resolved with 7167-x035 model printers

2.'48 column print' support is added for 7167, 7167series-2, 7168, 7168eries-2 and 7198 model printers.

Version 2.2.1 Release:

Fixed Issues:

1. Resolved an issue with performing MICR operation-Before it shows an error "Unknown Error"


Version 2.2.0 Release:

Fixed Issues:

1. NHPI communication supported. 


Version 2.1.0 Release:

Fixed Issues:

1. K59x and 7168SeriesII supports are added
2. Ethernet communication is provided.
3. F301 is changed to 7649_F301
4. Back lines tally is added for F309
5. ClearUserArea option is provided in following two options.
  A) ClearAllUserArea
  B) ClearUserDefinedArea 
6."IngnoreSynConfig" configuration option was added for 7167ser2 and 7197ser2 model printers.
7. Representation of 7167_5xxx and 7197_6xxx is changed to 7167_5xxx/6xxx and 7197_5xxx/6xxx respectively. 






