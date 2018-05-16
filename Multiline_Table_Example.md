# Multiline_Table

-----------------------------------------------------------------------------------------------------------------------------------------
CHANNEL PARAMETER VALUE ELIGIBLE FOR CJ COMMISSION WHEN TO USE IT
----------------------- -------------------------- --------------------------------------------------------------------------------------
CJ                      YES                        When the customer's last click was from a CJ affiliate link

DIRECT                  YES                        When the customer navigated directly to the advertiser's website
                                                   <aside class="notice">Important: Do not overwrite other channels with 'direct'. If
                                                   there is a click for another marketing channel before a user navigates directly to
                                                   the site, the 'channel' parameter must reflect that previous click.</aside>

AFFILIATE_OTHER         NO                         When the customer's last click was from an affiliate channel other than CJ

DISPLAY                 NO                         When the customer's last click was from a display campaign

SOCIAL                  NO                         When the customer's last click was from a social media campaign

SEARCH                  NO                         When the customer's last click was from a search campaign
                                                   * This is a test bullet
                                                   * This is another bullet

EMAIL                   NO                         When the customer's last click was from an email campaign

OTHER                   NO                         When the customer's last click was from a campaign not defined by the values above
-----------------------------------------------------------------------------------------------------------------------------------------


## Notes

Multiline tables allow headers and table rows to span multiple lines of text (but cells that span multiple columns or rows of the table are not supported).

These work like simple tables, but with the following differences:

- They must begin with a row of dashes, before the header text (unless the headers are omitted).
- They must end with a row of dashes, then a blank line.
- The rows must be separated by blank lines.

In multiline tables, the table parser pays attention to the widths of the columns, and the writers try to reproduce these relative widths in the output. So, if you find that one of the columns is too narrow in the output, try widening it in the Markdown source.
