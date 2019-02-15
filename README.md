# PPD File Xerox WorkCentre 6515
Postscript Printer Definition file to use Xerox WorkCentre 6515 printer on Linux with regular CUPS avoiding the Xerox Linux driver with awkward tooling and problems. For more information see: http://www.openprinting.org/printer/Xerox/Xerox-WorkCentre_6515DNI_MFP.

PPD is based on generic ppd file for Windows 10 x64.

- [PPD Download Link (unmodified)](https://www.support.xerox.com/support/workcentre-6515/file-download/enus.html?operatingSystem=win10x64&fileLanguage=en&contentId=142722&from=downloads&viewArchived=false)
- Version: 5.620.0.0

Tested on Fedora 29 x64.

## Modifications
Syntax:
- `*OpenGroup: PrintQuality/Print Quality/Color` to `*OpenSubGroup: PrintQuality/Print Quality/Color`
- `*CloseGroup: PrintQuality` to `*CloseSubGroup: PrintQuality`

Constraints:
- `*DefaultXRXOptionDuplex: False` to `*DefaultXRXOptionDuplex: True`

## Installation

Using CUPS web panel:

1. Make sure CUPS is installed on your system
2. Open http://localhost:631/admin
3. `Add Printer` (or modify existing printers)
4. Select Xerox model
5. Add PPD file from disk

Using system configuration:

Apart from the web panel of CUPS you can use the printer configuration tool provided by your distribution. It will usually configure the network printer according to definitions of a database, which didn't worked for the Xerox WorkCentre 6515 on Fedora Cinnamon x64. But after an initial configuration the configuration tools usually provide a possibility to use another PPD file as provided here.


