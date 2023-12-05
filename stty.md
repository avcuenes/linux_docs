# stty Command 

- The stty command sets certain I/O options for the device that is the current standard input. This command writes output to the device that is the current standard output.

## Usage

stty [-F DEVICE | --file=DEVICE] [SETTING]...
stty [-F DEVICE | --file=DEVICE] [-a|--all]
stty [-F DEVICE | --file=DEVICE] [-g|--save]

## Description

Mandatory arguments to long options are mandatory for short
options too.

-a, --all
        print all current settings in human-readable form

-g, --save
        print all current settings in a stty-readable form

-F, --file=DEVICE
        open and use the specified DEVICE instead of stdin

--help display this help and exit

--version
        output version information and exit

Optional - before SETTING indicates negation.  An * marks
non-POSIX settings.  The underlying system defines which settings
are available.


## Examples

``` stty --all ```
``` stty -F /dev/ttyUSB0 -a ```
``` stty -F /dev/ttyUSB0 -icanon -echo ```
``` stty -F /dev/ttyUSB0 (speed) 115200 ```

## References
1. <https://man7.org/linux/man-pages/man1/stty.1.html>
