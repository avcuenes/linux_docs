# Serial Ports 

### Display Serial Ports

If you want to display serial ports use this command;

```bash
ls /dev/tty*
```

This is what you see;

```bash
/dev/tty    /dev/tty14  /dev/tty20  /dev/tty27  /dev/tty33  /dev/tty4   /dev/tty46  /dev/tty52  /dev/tty59  /dev/tty8       /dev/ttyS12  /dev/ttyS19  /dev/ttyS25  /dev/ttyS31
/dev/tty0   /dev/tty15  /dev/tty21  /dev/tty28  /dev/tty34  /dev/tty40  /dev/tty47  /dev/tty53  /dev/tty6   /dev/tty9       /dev/ttyS13  /dev/ttyS2   /dev/ttyS26  /dev/ttyS4
/dev/tty1   /dev/tty16  /dev/tty22  /dev/tty29  /dev/tty35  /dev/tty41  /dev/tty48  /dev/tty54  /dev/tty60  /dev/ttyprintk  /dev/ttyS14  /dev/ttyS20  /dev/ttyS27  /dev/ttyS5
/dev/tty10  /dev/tty17  /dev/tty23  /dev/tty3   /dev/tty36  /dev/tty42  /dev/tty49  /dev/tty55  /dev/tty61  /dev/ttyS0      /dev/ttyS15  /dev/ttyS21  /dev/ttyS28  /dev/ttyS6
/dev/tty11  /dev/tty18  /dev/tty24  /dev/tty30  /dev/tty37  /dev/tty43  /dev/tty5   /dev/tty56  /dev/tty62  /dev/ttyS1      /dev/ttyS16  /dev/ttyS22  /dev/ttyS29  /dev/ttyS7
/dev/tty12  /dev/tty19  /dev/tty25  /dev/tty31  /dev/tty38  /dev/tty44  /dev/tty50  /dev/tty57  /dev/tty63  /dev/ttyS10     /dev/ttyS17  /dev/ttyS23  /dev/ttyS3   /dev/ttyS8
/dev/tty13  /dev/tty2   /dev/tty26  /dev/tty32  /dev/tty39  /dev/tty45  /dev/tty51  /dev/tty58  /dev/tty7   /dev/ttyS11     /dev/ttyS18  /dev/ttyS24  /dev/ttyS30  /dev/ttyS9

```

or if you wanna see some more details about the serial port you also use this command;

```bash
dmesg | grep tty
```

Also,If you wanna see live serial traffic at linux , you can use the following command;

```bash
dmesg -wH
```


## Differenece between
## Reference

1. <https://copyprogramming.com/howto/what-is-the-difference-between-ttys0-ttyusb0-and-ttyama0-in-linux>
2. <https://www.cyberciti.biz/faq/find-out-linux-serial-ports-with-setserial/>