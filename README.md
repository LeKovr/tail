# tail
The package is implemented using `tail` function provided by Linux. It simply reads the stdout of `tail` using `bufio.Scanner` and pass it to the application through a go channel.

## [LeKovr fork changes](https://github.com/LeKovr/tail)

Changed tail call arguments:
* removed "-c +1"
* "-F"  used instead "-f"
* added "-n" support (added argument to TailFile)

Also tests was simplified (takes 10 secs)
