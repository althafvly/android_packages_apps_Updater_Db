# PegasusOS OTA repo
In order for a device to be officially supported by PegasusOS, OTA information needs to be added.

## 1. Introduction ##
In order for a device to be OTA compliant, there are a few things to know.

### 1.1 JSON structure ###

```
{
  "response": [
    {
        "datetime": 1623675810,
        "filename": "marlin-ota_update-2021.06.14.21.zip",
        "id": "7a296f7e54b7406077b923ce59931b47",
        "romtype": "user",
        "size": 814462540,
        "url": "https://sourceforge.net/projects/pegasusandroid/files/marlin/11/marlin-ota_update-2021.06.14.21.zip/download",
        "version": "11"
    }
  ]
}
```

### 1.2 changelog.txt structure ### 
```
Highlights & Device Specific Changes:
Build type: user/userdebug/eng
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
