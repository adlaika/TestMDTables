``` {.table}
---
alignment: LLLL
header: true
markdown: true
table-width: 1.0
width: [0.11377245508982035, 0.0658682634730539, 0.2275449101796407, 0.592814371257485]
---
PARAMETER,REQUIRED,EXAMPLE,NOTES
CID,YES,CID=123456,"This value is set to the Enterprise ID, which is a static value provided
by CJ."
OID,YES,OID=145\_683-ABC,"The OID is a unique identifier, such as an order identifier or invoice
number, which must be populated for each order. It is used to reconcile
orders in the advertiser's system with CJ in order to validate each sale
or lead.

-   This value will be truncated after the 96th character
-   Only alphanumeric characters, dashes, and underscores can be
    included in the OID field
-   CJ prohibits the submission of personally identifiable information
    in the OID field, such as a full or partial email address
"
TYPE,YES,TYPE=5634,"This is a static value provided by CJ; it is also called an Action ID in
the Account Manager. Each account may have multiple actions and each
will be referenced by a different TYPE value."
AMOUNT,YES,AMOUNT=87.49,"The system assumes the AMOUNT= value is in the currency specified in the
CURRENCY parameter. If you specify a currency other than your functional
currency, the system converts the AMOUNT= value to an amount in your
functional currency using a current conversion rate.

The amount value should not include shipping or tax."
DISCOUNT,NO,DISCOUNT=12.99,"Discount parameter which enables you to apply a whole order discount to
a transaction.

An order which contain multiple items distributes the DISCOUNT value
throughout the items, based on the item amounts."
CURRENCY,YES,CURRENCY=USD,"Identifies the currency used to determine the AMT value for each item
involved in the action. This three-letter code is static and can be
hard-coded into the URL call for the image.

If a code is not specified, product prices display in the advertiser’s
functional currency. If a blank value is submitted (“CURRENCY=”, with no
specified value), a transaction error will occur.

For a list of supported currencies and codes, please visit the Support
Center."
COUPON,NO,COUPON=10off100,"Parameter for a coupon, voucher or discount code applied at the time of
purchase."
CONTAINER TAG ID,YES,,The unique identifier for the conversion tag.
NAME,YES,,"If you have multiple conversion tags, you can use this parameter to
uniquely identify your tags."
CHANNEL,NO,,"*Only use this parameter if instructed by your assigned CJ Client
Integration Engineer*

This parameter is where the advertiser passes the channel to which they
attribute the last click.

See the table below for acceptable values and their meanings."
CHANNEL\_TS,NO,CHANNEL\_TS=2017-02-14T22:16:46.623Z,"*Only use this parameter if instructed by your assigned CJ Client
Integration Engineer*

This parameter is where the advertiser passes the date/time stamp for
the last click that they are attributing the transaction to. They must
use this format: NOTES: \* format: yyyy-mm-ddThh24:mm:ss.sssZ \* all
dates and times must be in UTC \* the .toISOString() method in
javaScript to produces this format \* this is the only format CJ's
system will accept"
```
