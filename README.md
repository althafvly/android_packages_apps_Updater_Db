# PegasusOS OTA repo
In order for a device to be officially supported by PegasusOS, OTA information needs to be added.

## 1. Introduction ##
In order for a device to be OTA compliant, there are a few things to know.

### 1.1 JSON structure ###

```
{
  "response": [
    {
      "datetime": 1230764400,
      "filename": "ota-package.zip",
      "id": "5eb63bbbe01eeed093cb22bb8f5acdc3",
      "romtype": "unofficial",
      "size": 314572800,
      "url": "https://example.com/ota-package.zip",
      "version": "11"
    }
  ]
}
```

## 2 Guidelines ##
* Check if manufacturer is already existing
* Check if published link is official
* Check if JSON is intact with help of online validator tools like [https://jsonformatter.curiousconcept.com](https://jsonformatter.curiousconcept.com) or [https://jsonformatter.org](https://jsonformatter.org)
* Check if no extra / missing spaces
