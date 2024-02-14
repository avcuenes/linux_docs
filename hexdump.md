# hexdump Command

- hexdump - display file contents in hexadecimal, decimal, octal,
       or ascii
- The hexdump utility is a filter which displays the specified
       files, or standard input if no files are specified, in a
       user-specified format.

## Options
Below, the length and offset arguments may be followed by the
       multiplicative suffixes KiB (=1024), MiB (=1024*1024), and so on
       for GiB, TiB, PiB, EiB, ZiB and YiB (the "iB" is optional, e.g.,
       "K" has the same meaning as "KiB"), or the suffixes KB (=1000),
       MB (=1000*1000), and so on for GB, TB, PB, EB, ZB and YB.

       -b, --one-byte-octal
           One-byte octal display. Display the input offset in
           hexadecimal, followed by sixteen space-separated,
           three-column, zero-filled bytes of input data, in octal, per
           line.

       -X, --one-byte-hex
           One-byte hexadecimal display. Display the input offset in
           hexadecimal, followed by sixteen space-separated, two-column,
           zero-filled bytes of input data, in hexadecimal, per line.

       -c, --one-byte-char
           One-byte character display. Display the input offset in
           hexadecimal, followed by sixteen space-separated,
           three-column, space-filled characters of input data per line.

       -C, --canonical
           Canonical hex+ASCII display. Display the input offset in
           hexadecimal, followed by sixteen space-separated, two-column,
           hexadecimal bytes, followed by the same sixteen bytes in %_p
           format enclosed in | characters. Invoking the program as hd
           implies this option.

       -d, --two-bytes-decimal
           Two-byte decimal display. Display the input offset in
           hexadecimal, followed by eight space-separated, five-column,
           zero-filled, two-byte units of input data, in unsigned
           decimal, per line.

       -e, --format format_string
           Specify a format string to be used for displaying data.

       -f, --format-file file
           Specify a file that contains one or more newline-separated
           format strings. Empty lines and lines whose first non-blank
           character is a hash mark (#) are ignored.

       -L, --color[=when]
           Accept color units for the output. The optional argument when
           can be auto, never or always. If the when argument is
           omitted, it defaults to auto. The colors can be disabled; for
           the current built-in default see the --help output. See also
           the Colors subsection and the COLORS section below.

       -n, --length length
           Interpret only length bytes of input.

       -o, --two-bytes-octal
           Two-byte octal display. Display the input offset in
           hexadecimal, followed by eight space-separated, six-column,
           zero-filled, two-byte quantities of input data, in octal, per
           line.

       -s, --skip offset
           Skip offset bytes from the beginning of the input.

       -v, --no-squeezing
           The -v option causes hexdump to display all input data.
           Without the -v option, any number of groups of output lines
           which would be identical to the immediately preceding group
           of output lines (except for the input offsets), are replaced
           with a line comprised of a single asterisk.

       -x, --two-bytes-hex
           Two-byte hexadecimal display. Display the input offset in
           hexadecimal, followed by eight space-separated, four-column,
           zero-filled, two-byte quantities of input data, in
           hexadecimal, per line.

       -h, --help
           Display help text and exit.

       -V, --version
           Print version and exit.

       For each input file, hexdump sequentially copies the input to
       standard output, transforming the data according to the format
       strings specified by the -e and -f options, in the order that
       they were specified.

## Examples
hexdump -C /dev/ttyUSB0
hexdump -n [wanted byte len] /dev/ttyUSB0
hexdump -v /dev/ttyUSB0

## References
1. <https://man7.org/linux/man-pages/man1/hexdump.1.html>
2. <https://www.geeksforgeeks.org/hexdump-command-in-linux-with-examples/>