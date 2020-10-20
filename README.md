# Fargo Public Library Koha notices

These are the notice templates for the Fargo Public Library's Koha system using template toolkit. 

## Issue Quick Slip

ISSUEQSLIP cycles through all checkouts and displays items that were checked-out today. It checks renewals and creates a section for renewals if there are any. It also checks if the record has holds or is non-renewable and displays an appropriate message.

Finally, it cycles through checkouts and renewals and totals the items' replacement prices to show the user how much they saved by using the library.

## Item Due Today

The DUEDGST cycles through all checkouts and displays items that are due today. It also checks to see if the records have holds or are non-renewable and displays an appropriate message.

## Overdue and Second Overdue

ODUE.tt and secondnotice.tt cycle through overdues for anything 10 or 20 days overdue, respectively. It's important that the amount overdue (in the case of these -10 and -20 days) match exactly the days in **Overdue notice/status triggers** (overduerules.pl). This notice is triggered by Koha and if they do not match, it may not show the right overdue items. This notice also checks for overdues *not* triggered and lists them seperately if so. Also includes logic to check if the item can be renewed.

## Bill

Similar to ODUE.tt, but includes replacement price. The trigger time must match the third trigger in **Overdue notice/status triggers** (overduerules.pl). Also includes logic to check if the item can be renewed.

## TODO

1. Clean up styles to use the ```NoticeCSS``` syspref.
