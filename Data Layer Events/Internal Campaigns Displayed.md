# Internal Campaigns Displayed

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Internal Campaigns Displayed",
    "airTravel": {
        "bookingInteraction": "<bookingInteraction>"
    },
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
|airTravel.bookingInteraction|string|Captures the various interactions within the Trip Booking flow. |Flight Search Performed, Flight Listing Displayed, Flight Summary Displayed, Guest Info Form Displayed, Flight Segment Seat Map Displayed|||||||
|internalCampaign.campaignList[n].internalCampaignID|string|Unique Identifier of an internal campaign|2345, 56789, 9876|||||||




