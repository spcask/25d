September 2016: Read Beej's Guide to Network Programming
========================================================
About 10 years ago, I came across a very entertaining book about network
programming in C called [*Beej's Guide to Network Programming*][BGNET]
by Brian "Beej Jorgensen" Hall.

Recently I found that the guide was updated for IPv6 (Version 3.0.21,
June 8, 2016). I decided to download the latest guide and study it to
learn the modern way of writing network programming code that works for
both IPv4 and IPv6.

I performed several experiments and wrote several example programs while
reading this guide. They can be found at
<https://github.com/susam/lab/tree/master/c/beej-guide-to-network-programming>.

The experiments performed while reading this guide led to two
StackOverflow questions.

  1. [Why can a client receive messages after shutdown(sockfd, SHUT_RD)?][SO1]
  2. [Why is netcat unable to receive the second broadcast message?][SO2]

[BGNET]: http://beej.us/guide/bgnet/
[SO1]: http://stackoverflow.com/q/39698037/303363
[SO2]: http://stackoverflow.com/q/40194933/303363


Contents
--------
* [Introduction](#readme)
* [Progress log](#progress-log)


Progress Log
------------
The list below shows how much time I spent each day in reading and
experimenting with concepts learnt from the book. The comment column
shows the pages and sections read each day.

    Day  Date        Time   Comment
    ---  ----------  -----  --------------------------------------------
    01   2016-09-01  0.5 h  01-06: 1.1-1.9, 2.1-2.2
    02   2016-09-02  0.5 h  07-12: 3.1-3.3
    03   2016-09-12  1.0 h  12-14: 3.4, 4
    04   2016-09-13  1.5 h  15-17: 5.1
    05   2016-09-18  1.5 h  18: 5.2
    06   2016-09-19  2.5 h  18-20: 5.3-5.4
    07   2016-09-20  2.0 h  20-22: 5.5-5.7
    08   2016-09-23  2.0 h  22-23: 5.8
    09   2016-09-28  1.5 h  23-24: 5.9
    10   2016-10-02  1.0 h  24: 5.10-5.11
    11   2016-10-03  2.0 h  25-27: 6.1
    12   2016-10-04  2.0 h  27-32: 6.2-6.3
    13   2016-10-07  1.0 h  33: 7.1
    14   2016-10-12  1.0 h  33-35: 7.2
    15   2016-10-13  2.0 h  35-38: 7.2
    16   2016-10-14  0.5 h  38-39: 7.3
    17   2016-10-15  1.0 h  39-41: 7.4
    18   2016-10-17  1.5 h  41-42: 7.4
    19   2016-10-19  1.0 h  43-45: 7.4
    20   2016-10-20  1.5 h  45-50: 7.4
    21   2016-10-22  1.5 h  50-54: 7.5-7.6
    22   2016-10-23  1.5 h  55-70: 8, 9.1-9.6
    23   2016-10-25  1.0 h  71-75: 8, 9.7-9.10
    24   2016-10-26  1.5 h  76-82: 9.11-9.16
    25   2016-10-27  2.0 h  83-99: 9.17-9.24, 10.1-10.3

         Total      34.5 h
         Average     1.4 h/d
