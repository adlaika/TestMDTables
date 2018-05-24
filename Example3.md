+-------+---+---------------+-----------------------------------------+
| PARAM | R | EXAMPLE       | NOTES                                   |
| ETER  | E |               |                                         |
|       | Q |               |                                         |
|       | U |               |                                         |
|       | I |               |                                         |
|       | R |               |                                         |
|       | E |               |                                         |
|       | D |               |                                         |
+:======+:==+:==============+:========================================+
| CID   | Y | CID=123456    | This value is set to the Enterprise ID, |
|       | E |               | which is a static value provided by CJ. |
|       | S |               |                                         |
+-------+---+---------------+-----------------------------------------+
| OID   | Y | OID=145\_683- | The OID is a unique identifier, such as |
|       | E | ABC           | an order identifier or invoice number,  |
|       | S |               | which must be populated for each order. |
|       |   |               | It is used to reconcile orders in the   |
|       |   |               | advertiser's system with CJ in order to |
|       |   |               | validate each sale or lead.             |
|       |   |               |                                         |
|       |   |               | -   This value will be truncated after  |
|       |   |               |     the 96th character                  |
|       |   |               | -   Only alphanumeric characters,       |
|       |   |               |     dashes, and underscores can be      |
|       |   |               |     included in the OID field           |
|       |   |               | -   CJ prohibits the submission of      |
|       |   |               |     personally identifiable information |
|       |   |               |     in the OID field, such as a full or |
|       |   |               |     partial email address               |
+-------+---+---------------+-----------------------------------------+
| TYPE  | Y | TYPE=5634     | This is a static value provided by CJ;  |
|       | E |               | it is also called an Action ID in the   |
|       | S |               | Account Manager. Each account may have  |
|       |   |               | multiple actions and each will be       |
|       |   |               | referenced by a different TYPE value.   |
+-------+---+---------------+-----------------------------------------+
| AMOUN | Y | AMOUNT=87.49  | The system assumes the AMOUNT= value is |
| T     | E |               | in the currency specified in the        |
|       | S |               | CURRENCY parameter. If you specify a    |
|       |   |               | currency other than your functional     |
|       |   |               | currency, the system converts the       |
|       |   |               | AMOUNT= value to an amount in your      |
|       |   |               | functional currency using a current     |
|       |   |               | conversion rate.                        |
|       |   |               |                                         |
|       |   |               | The amount value should not include     |
|       |   |               | shipping or tax.                        |
+-------+---+---------------+-----------------------------------------+
| DISCO | N | DISCOUNT=12.9 | Discount parameter which enables you to |
| UNT   | O | 9             | apply a whole order discount to a       |
|       |   |               | transaction.                            |
|       |   |               |                                         |
|       |   |               | An order which contain multiple items   |
|       |   |               | distributes the DISCOUNT value          |
|       |   |               | throughout the items, based on the item |
|       |   |               | amounts.                                |
+-------+---+---------------+-----------------------------------------+
| CURRE | Y | CURRENCY=USD  | Identifies the currency used to         |
| NCY   | E |               | determine the AMT value for each item   |
|       | S |               | involved in the action. This            |
|       |   |               | three-letter code is static and can be  |
|       |   |               | hard-coded into the URL call for the    |
|       |   |               | image.                                  |
|       |   |               |                                         |
|       |   |               | If a code is not specified, product     |
|       |   |               | prices display in the advertiser’s      |
|       |   |               | functional currency. If a blank value   |
|       |   |               | is submitted (“CURRENCY=”, with no      |
|       |   |               | specified value), a transaction error   |
|       |   |               | will occur.                             |
|       |   |               |                                         |
|       |   |               | For a list of supported currencies and  |
|       |   |               | codes, please visit the Support Center. |
+-------+---+---------------+-----------------------------------------+
| COUPO | N | COUPON=10off1 | Parameter for a coupon, voucher or      |
| N     | O | 00            | discount code applied at the time of    |
|       |   |               | purchase.                               |
+-------+---+---------------+-----------------------------------------+
| CONTA | Y |               | The unique identifier for the           |
| INER  | E |               | conversion tag.                         |
| TAG   | S |               |                                         |
| ID    |   |               |                                         |
+-------+---+---------------+-----------------------------------------+
| NAME  | Y |               | If you have multiple conversion tags,   |
|       | E |               | you can use this parameter to uniquely  |
|       | S |               | identify your tags.                     |
+-------+---+---------------+-----------------------------------------+
| CHANN | N |               | *Only use this parameter if instructed  |
| EL    | O |               | by your assigned CJ Client Integration  |
|       |   |               | Engineer*                               |
|       |   |               |                                         |
|       |   |               | This parameter is where the advertiser  |
|       |   |               | passes the channel to which they        |
|       |   |               | attribute the last click.               |
|       |   |               |                                         |
|       |   |               | See the table below for acceptable      |
|       |   |               | values and their meanings.              |
+-------+---+---------------+-----------------------------------------+
| CHANN | N | CHANNEL\_TS=2 | *Only use this parameter if instructed  |
| EL\_T | O | 017-02-14T22: | by your assigned CJ Client Integration  |
| S     |   | 16:46.623Z    | Engineer*                               |
|       |   |               |                                         |
|       |   |               | This parameter is where the advertiser  |
|       |   |               | passes the date/time stamp for the last |
|       |   |               | click that they are attributing the     |
|       |   |               | transaction to. They must use this      |
|       |   |               | format: NOTES: \* format:               |
|       |   |               | yyyy-mm-ddThh24:mm:ss.sssZ \* all dates |
|       |   |               | and times must be in UTC \* the         |
|       |   |               | .toISOString() method in javaScript to  |
|       |   |               | produces this format \* this is the     |
|       |   |               | only format CJ's system will accept     |
+-------+---+---------------+-----------------------------------------+


