# nm command

The nm command displays information about symbols in the specified File, which can be an object file, an executable file, or an object-file library.
If the file contains no symbol information, the nm command reports the fact, but does not interpret it as an error condition. The nm command reports numerical values in decimal notation by default.

## Examples
To list the static and external symbols of the object file a.out, enter:
``` bash
nm -e a.out
```
To display symbol sizes and values as hexadecimal and sort the symbols by value, enter:
```bash
nm -xv a.out
```

To display symbol of all 64-bit objects in libc.a, ignoring all 32-bit objects:
```bash
nm -X64 /usr/lib/libc.a
```

## References
1.<https://www.ibm.com/docs/en/aix/7.2?topic=n-nm-command>
