# Windows 10 Enterprise LTSC Install Guide
<img align="right" width="300" height="300" src="https://files.catbox.moe/dutpxu.webp">

> A guide to installing Windows 10 Enterprise on a Boot Drive


Windows 10 Enterprise LTSC (Long-Term Servicing Channel) is a long-term 
support variant of Windows 10 used by Corporations released every 2 to 3 years. 
Each release is supported with security updates for either 5 or 10 years after its release.
It's primarily used in bigger companies (as the name suggests) which rely on it's stability and longevity.

## How To Install

- [Rufus](https://rufus.ie/en/)
- [USB 8gb+](https://amzn.eu/d/483SMH7)
- [Windows10Enterprise ISO](https://rentry.co/notwindows)
- [MAS](https://github.com/massgravel/Microsoft-Activation-Scripts/archive/refs/heads/master.zip) (Microsoft Activation Tool)

### Windows Setup. 
Flash the ISO onto the USB Drive using Rufus,
it should look like this ->

<img align="Right" width="474" height="650" src="https://files.catbox.moe/pusvrb.png">

> [!IMPORTANT]
> Some older Motherboards will be set to "LEGACY" Mode.
> Open windows search, type "msinfo" and find the Line "BIOS Mode" It's either UEFI or Legacy. Rufus needs to show UEFI/Legacy


1. Reboot into BIOS
3. Select USB as Boot Drive 1#
4. Disconnect your Ethernet Cable from the Device
5. Set Up Windows like Normal
6. *DO NOT* enter Wifi Info, choose limited Setup without Internet and make a Local Account

### Activate License

Use MAS Tool from the Download or copy-paste the 
following text into
Powershell. 

``irm https://massgrave.dev/get | iex``

Once opened, Select "1". It should be
activating Windows License for Windows Enterprise.

Close after it's done.
