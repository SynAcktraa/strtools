# toString Converter

>A terminal based program to convert base numbers to string.

## Help:

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

---

### Binary to String↴

```bash
./toString -bd -f bin.txt
```

Output:

```nani
I use arch btw thank you.
```
___
### Octal to String↴

```bash
./toString -od -f octal.txt
```

Output:

```nani
Why don't jokes work in octal? Because 7 10 11.
```
___
### Hexadecimal to String↴

```bash
./toString -hd -i "53 74 61 72 20 74 68 69 73 20 70 72 6f 6a 65 63 74 20 3a 29"
```

Output:

```nani
Star this project :)
```
___
### Decimal to String↴

```bash
./toString -id -i "72 97 118 101 32 97 32 110 105 99 101 32 100 97 121 32 40 59"
```

Output:

```nani
Have a nice day (;
```

---
___

### Redirecting output to a file:
---

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

___

`Note: It still doesn't check if the value you are providing is correct. Don't worry :), I'm working on it.`