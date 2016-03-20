# barf
Block Apache Request Floods

Source: http://www.webhostingtalk.com/showthread.php?t=949636&p=6806550#post6806550

```
##############################################################################
#   _                 __
#  | |               / _|   BLOCK
#  | |__   __ _ _ __| |_    APACHE
#  | '_ \ / _` | '__|  _|   REQUEST
#  | |_) | (_| | |  | |     FLOODS
#  |_.__/ \__,_|_|  |_|      LoL:D
#
##############################################################################

##############################################################################
#
#  Block an IP address if it issues x number of y requests
#  to apache within z seconds. This script takes 4 options:
#
#  example.com  this is the domain to monitor
#  -n <num>     if this many requests
#  -t <num>     are made within this many seconds
#  -s <req>     for this string
#               then the IP address issuing the requests will be blocked.
#
#  Examples:
#
#    Look for 3 requests within 10 seconds that match GET /index.php
#    ./script example.com -n 3 -t 10 -s "GET /index.php"
#
#    Look for 10 requests within 30 seconds that match GET / HTTP/1.1
#    ./script example.com -n 10 -t 30 -s "GET / HTTP/1.1"
#
#  This is the expected Apache log format, which is the default on cPanel servers:
#  1.2.3.4 - - [28/Jun/2009:16:43:05 -0400] "GET / HTTP/1.1" 404 - "-" "-"
#
##############################################################################

```
