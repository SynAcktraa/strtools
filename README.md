# toString Converter

>A terminal based program to convert base numbers to string.

## **Help↴**

>toString -h

Output:

```nani

Usage: toString.exe <type> <input> data|file -o outfile.txt

|CLI options|:-
   type:
      -od = The data passed should be octal.
      -bd = The data passed should be binary.
      -id = The data passed should be decimal.
      -hd = The data passed should be hexadecimal.

   input:
      -i = takes next argument as data string.
      -f = takes next argument as filename.

   optional:
      -o = takes next argument as filename.
           (if filename is null, it's set to toString_out as filename.)
           [if '-o' is not used, result is printed to STDOUT.]

```

#

### **Binary to String ↴**

```bash
./toString -bd -f bin.txt
```

Output:

<pre>
I use arch btw thank you.
</pre>

#
### **Octal to String ↴**

```bash
./toString -od -f octal.txt
```

Output:

<pre>
<a target="_blank" href="https://www.youtube.com/watch?v=GBIIQ0kP15E">https://www.youtube.com/watch?v=GBIIQ0kP15E</a>
</pre>

#
### **Hexadecimal to String ↴**

```bash
./toString -hd -i "53 74 61 72 20 74 68 69 73 20 70 72 6f 6a 65 63 74 20 3a 29"
```

Output:

<pre>
Star this project :)
</pre>
#
### **Decimal to String ↴**

```bash
./toString -id -i "72 97 118 101 32 97 32 110 105 99 101 32 100 97 121 32 40 59"
```

Output:

<pre>
Have a nice day (;
</pre>

#
#

### **Redirecting output to a file:**
#

##### Using the redirection operator↴

```bash
./toString -hd -i "63 6f 6f 6c 20 73 68 69 74" > hex_out.txt
```

##### Using the -o argument with a filename↴

```bash
./toString -od -i "143 157 156 164 162 151 142 165 164 145 40 72 51" -o oct_out
```

##### Using the -o argument without a filename↴

```bash
./toString -id -i "105 100 107 32 105 100 99 46" -o
```
>ps: "-o" without a parameter uses the default filename 'toString_out'

## **License**

### <a target="_blank" href="https://choosealicense.com/licenses/mit/">MIT</a>

Copyright for portions of project [toString-Converter](https://github.com/SynAcktraa/toString-Converter) are held by [Github Account [SynAcktraa](https://github.com/SynAcktraa) Owner, 2022] as part of project [toString-Converter](https://github.com/SynAcktraa/toString-Converter)

All other copyright for project [toString-Converter](https://github.com/SynAcktraa/fromString-Converter) are held by [Github Account [SynAcktraa](https://github.com/SynAcktraa) Owner, 2022].

Check the [LICENSE](LICENSE) for more details.