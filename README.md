# Fargo Public Library Koha notices

These are the notice templates for the Fargo Public Library's Koha system using template toolkit. 

## Issue Quick Slip

ISSUEQSLIP cycles through all checkouts and displays items that were checked-out today. It checks renewals and creates a section for renewals if there are any. It also checks if the record has holds or is non-renewable and displays an appropriate message.

Finally, it cycles through checkouts and renewals and totals the items' replacement prices to show the user how much they saved by using the library.

## Item Due Today

The DUEDGST cycles through all checkouts and displays items that are due today. It also checks to see if the records have holds or are non-renewable and displays an appropriate message.

## TODO

1. Clean up styles to use the ```NoticeCSS``` syspref.
