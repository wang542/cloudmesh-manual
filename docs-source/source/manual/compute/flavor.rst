flavor
======

.. parsed-literal::

    Usage:
        flavor list [NAMES] [--cloud=CLOUD] [--refresh] [--output=OUTPUT]


    Options:
       --output=OUTPUT  the output format [default: table]
       --cloud=CLOUD    the ycloud name
       --refresh        refreshes the data before displaying it

    Description:

        This lists out the flavors present for a cloud

    Examples:
        cm flavor list --refresh
        cm flavor list
        cm flavor list --output=csv
        cm flavor list 58c9552c-8d93-42c0-9dea-5f48d90a3188 --refresh

        please remember that a uuid or the flavor name can be used to
        identify a flavor.

Timer: 0.0000s (man flavor --format=rst)
