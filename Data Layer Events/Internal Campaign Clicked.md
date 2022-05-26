# Internal Campaign Clicked

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Internal Campaign Clicked",
    "CustomArray": [
        {
            "ds6": <ds6>
        }
    ],
    "internalCampaign": {
        "campaignList": [
            {
                "internalCampaignID": "<internalCampaignID>"
            }
        ]
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|CustomArray[n].ds6|integer|Stan Custom DS 6||||||||
|internalCampaign.campaignList[n].internalCampaignID|string|Unique Identifier of an internal campaign|2345, 56789, 9876|||||||




