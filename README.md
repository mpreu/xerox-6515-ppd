# PPD File Xerox WorkCentre 6515
Postscript Printer Definition file to use Xerox WorkCentre 6515 printer on Linux with regular CUPS avoiding the Xerox Linux driver with awkward tooling and problems. For more information see: http://www.openprinting.org/printer/Xerox/Xerox-WorkCentre_6515DNI_MFP

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