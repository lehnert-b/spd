# spd

Create random pseudonyms for sensitive research data - *s*hare *p*seudonymized *d*ata.

spd is
- a command line tool (no graphical user interface for the time being)
- developed on Windows but should run on any system supported by the go language (please try it out and report!)
- free and open source under the GNU GPL
- meant for researchers in medicine or social sciences or psychology or any field in which they are obligated (by law or ethics) to pseudonymize data.
- worth a try even if it is in no way, shape or form perfect. This is a project starting out.

Executable files can be found as "Release" under https://github.com/lehnert-b/spd/releases

A short introduction video is on https://youtu.be/zgKoUX2DUHA

Please read the PDF file for instructions of how to use the programm: https://github.com/lehnert-b/spd/blob/main/spd%20Description%20and%20Manual.pdf


## Examples
To produce `500` pseudonyms for a study called "`ABC`" in a file `pseudo.csv` call it as

```
spd -n 500 -pre ABC -out pseudo.csv
```

To get longer pseudonyms so they are less likely to be remembered by humans and you want them to be printed on the console (stdout) call is as

```
spd -n 20 -l 50 -v
```

If you have a file of semicolon separated data in `test3.csv`and you want an extra column with pseudonyms added to each line under the header of `new_id` call `spd` as

```
spd -in test3.csv -sep=";" -head new_id -out test3_p.csv
```

More instructions and examples are in the Manual https://github.com/lehnert-b/spd/blob/main/spd%20Description%20and%20Manual.pdf

