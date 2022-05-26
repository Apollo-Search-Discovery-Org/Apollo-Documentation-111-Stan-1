# Custom Event 4

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Custom Event 4",
    "customTP3": [
        {
            "ds3": {
                "1": <1>
            }
        }
    ],
    "eventDetails": {
        "checkoutStep": "<checkoutStep>"
    },
    "wishlist": {
        "total": {
            "value": "<value>"
        }
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|customTP3[n].ds3.1|boolean|Stan Custom DS 3.1||||||||
|eventDetails.checkoutStep|string|Describes a discrete step in the checkout flow. |Cart Review, Billing Info, Shipping Info, Order Review|||||||
|wishlist.total.value|string|String representation of the total value of all products in a wishlist. Positive. Up to two decimal places for cents. No currency symbol.|5, 20, 10.22|^[0-9]*(\.[0-9]{1,2})?$||||||




