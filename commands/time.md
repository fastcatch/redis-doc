@complexity O(1)


The `TIME` command returns the current server time as a two items lists: an unix timestamp and the amount of microseconds already elapsed in the current second.
Basically the interface is very similar to the one of the `gethostbyname` syscall.

@return

@multi-bulk-reply, specifically:

A multi bulk reply containing two elements:
* unix time in seconds.
* microseconds.

@examples

    @cli
    TIME
    TIME