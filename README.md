# PegasusOS OTA repo
In order for a device to be officially supported by PegasusOS, OTA information needs to be added.

## 1. Introduction ##
In order for a device to be OTA compliant, there are a few things to know.

### 1.1 JSON structure ###

```
{
  "response": [
    {
        "maintainer": "Name (nickname)",
        "oem": "OEM",
        "device": "Device Name",
        "filename": "PegasusOS-11.0-<date>-<device codename>.zip",
        "download": "https://sourceforge.net/projects/pegasusandroid/files/<device codename>/<androidversion>/PegasusOS-11.0-<date>-<device codename>.zip/download",
        "timestamp": 0000000000,
        "md5": "abcdefg123456",
        "size": 123456789,
        "version": "<androidversion>",
        "buildtype": "Testing/Alpha/Beta/Weekly/Monthly",
        "forum": "https://forum link",
        "gapps": "https://gapps link",
        "firmware": "https://firmware link",
        "modem": "https://modem link",
        "bootloader": "https://bootloader link",
        "recovery": "https://recovery link",
        "paypal": "https://donation link",
        "telegram": "https://telegram link"
    }
  ]
}
```

### 1.2 changelog.txt structure ### 
```
Highlights & Device Specific Changes:
Build type: Testing/Alpha/Beta/Weekly/Monthly
Device: Device name (<device codename>)
Device maintainer: Name (nickname)
Required firmware: add if any else remove this line

===== <date> =====
- change 1
- change 2
- change 3
```

## 2 Guidelines ##
* Check if manufacturer is already existing
* Check if published link is official
* Check if JSON is intact with help of online validator tools like [https://jsonformatter.curiousconcept.com](https://jsonformatter.curiousconcept.com) or [https://jsonformatter.org](https://jsonformatter.org)
* Check if no extra / missing spaces
