# Multiline_Table

+-------------------------+----------------------------+-------------------------------------------------------------------------------------+
| CHANNEL PARAMETER VALUE | ELIGIBLE FOR CJ COMMISSION | WHEN TO USE IT                                                                      |
+:========================+:===========================+:====================================================================================+
| CJ                      | YES                        | When the customer's last click was from a CJ affiliate link                         |
+-------------------------+----------------------------+-------------------------------------------------------------------------------------+
| DIRECT                  | YES                        | When the customer navigated directly to the advertiser's website                    |
|                         |                            |                                                                                     |
|                         |                            | <aside class="notice">Important: Do not overwrite other channels with 'direct'. If  |
|                         |                            | there is a click for another marketing channel before a user navigates directly to  |
|                         |                            | the site, the 'channel' parameter must reflect that previous click.</aside>         |
+-------------------------+----------------------------+-------------------------------------------------------------------------------------+
| AFFILIATE_OTHER         | NO                         | When the customer's last click was from an affiliate channel other than CJ          |
+-------------------------+----------------------------+-------------------------------------------------------------------------------------+
| DISPLAY                 | NO                         | When the customer's last click was from a display campaign                          |
+-------------------------+----------------------------+-------------------------------------------------------------------------------------+
| SOCIAL                  | NO                         | When the customer's last click was from a social media campaign                     |
+-------------------------+----------------------------+-------------------------------------------------------------------------------------+
| SEARCH                  | NO                         | When the customer's last click was from a search campaign                           |
|                         |                            |                                                                                     |
|                         |                            | * This is a test bullet                                                             |
|                         |                            | * This is another bullet                                                            |
+-------------------------+----------------------------+-------------------------------------------------------------------------------------+
| EMAIL                   | NO                         | When the customer's last click was from an email campaign                           |
+-------------------------+----------------------------+-------------------------------------------------------------------------------------+
| OTHER                   | NO                         | When the customer's last click was from a campaign not defined by the values above  |
+-------------------------+----------------------------+-------------------------------------------------------------------------------------+

## Notes

The row of =s separates the header from the table body, and can be omitted for a headerless table. The cells of grid tables may contain arbitrary block elements (multiple paragraphs, code blocks, lists, etc.). Cells that span multiple columns or rows are not supported. Grid tables can be created easily using [Emacs table mode](http://table.sourceforge.net/).

Alignments can be specified as with pipe tables, by putting colons at the boundaries of the separator line after the header.

For headerless tables, the colons go on the top line instead.
