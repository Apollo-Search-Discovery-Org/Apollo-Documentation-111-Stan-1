# Order Placed

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Order Placed",
    "cart": {
        "cartID": "<cartID>"
    },
    "customTP3": [
        {
            "ds3": {
                "1": <1>
            }
        }
    ],
    "transaction": {
        "item": [
            {
                "altPersonPickUp": <altPersonPickUp>,
                "ds3": {
                    "2": <2>
                },
                "fulfillment": {
                    "method": "<method>",
                    "source": "<source>"
                },
                "price": {
                    "sellingPrice": "<sellingPrice>"
                },
                "productInfo": {
                    "productID": "<productID>"
                },
                "quantity": <quantity>,
                "shippingAddress": {
                    "country": "<country>",
                    "postalCode": "<postalCode>"
                }
            }
        ],
        "purchaseID": "<purchaseID>",
        "total": {
            "currency": "<currency>"
        }
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|cart.cartID|string|Back-end identifier for a shopping cart|12345, 435678, 34567, XCV456, XCV876|||||||
|customTP3[n].ds3.1|boolean|Stan Custom DS 3.1||||||||
|transaction.item[n].altPersonPickUp|integer|When a user has put in the information of an alternate pick up person during the checkout process.||||||||
|transaction.item[n].ds3.2|number|Stan Custom DS TP 3.2||||||||
|transaction.item[n].fulfillment.method|string|Describes the method of fulfillment|Shipped, Emailed, Pick Up In Store, Will Call|||||||
|transaction.item[n].fulfillment.source|string|Describes the entity responsible for fulfillment. Uasge is flexible.|Vendor:xyz, Store:43567, Email:system3, Warehouse:7865|||||||
|transaction.item[n].price.sellingPrice|string|String representation of the price paid after coupons or discounts. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|transaction.item[n].productInfo.productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|transaction.item[n].quantity|integer|Integer number of products being acted upon \(added to a cart, removed from wishlist, purchased, reserved\)|1, 2, 3, 4, 5||||1|||
|transaction.item[n].shippingAddress.country|string|Indicates the country of the address of the shipment. ISO 3166 \(alpha-2\) Uppercase.|US, CA, FR, UK|^[A-Z]{2}$||||||
|transaction.item[n].shippingAddress.postalCode|string|The mailing zip or postal code associated with the address of the shipment. |53533, 30381, M1R 0E9, M3C 0C1|||||||
|transaction.purchaseID|string|Unique identifier of the purchase. Max Length 20. Used as Unique ID of the purchase or deduplication.|ABC-132456789, DEF-132456789, 0987654567|^[a-zA-Z0-9]{6,20}$|6|20||||
|transaction.total.currency|string|Currency of the transaction. ISO 4217 \(3 character alpha\), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||




