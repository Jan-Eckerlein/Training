# IPv6 Subnetting

[Aufgabe](https://bkes-hamm.de/iserv/fs/file/local/Groups/Klasse%20ITB2/FRA/EVP-LF9%20-%20Netzwerke%20und%20Dienste%20bereitstellen/LS%209.1%20-%20Routing/IPv6-Subnetting%20-%20AB1.pdf)

## Aufgabe 1

Ihre Firma hat vom ISP das Netz 3FFA:FF2B:4D:A000::/51 zugewiesen bekommen. Teilen  
Sie dieses Netz in 4 Subnetze auf.

0000 0000

000 0 0000

101<mark>0 0</mark> 000

- 1010 0000 | A0

- 1010 1000 | A8

- 1011 0000 | B0

- 1011 1000 | B8

vier Subnetze:

- 3FFA:FF2B:004D:A000:0000:0000/53

- 3FFA:FF2B:004D:A800:0000:0000/53

- 3FFA:FF2B:004D:B000:0000:0000/53

- 3FFA:FF2B:004D:B800:0000:0000/53

```mermaid
graph TD;

a(3FFA:FF2B:4D:A000::/51)-->|Hexadezimal ausschreiben|b(3FFA:FF2B:004D:A000:0000:0000/51)
a-->|4 subnetzte|c(2bit)
c-->|präfix ausrechnen|d(/53)
```


## Aufgabe 2

```mermaid
graph TD;

a(3FFA:FF2B:4D:A000::/51)
a-->|ausschreiben|b(3FFA:FF2B:004D:A000:0000:0000/51)
a-->|bitzahl für 16 subnets|c(4 bit)
b-->|grenzbereich ermitteln|d(3FFA:FF2B:004D:<mark>A0</mark>00:0000:0000)
d-->e(A0)
e-->|ausschreiben|f(101<mark>0 000</mark>0)
f-->|variationen|g(000<mark>0 000</mark>0  -  00<br>000<mark>0 001</mark>0  -  02<br>000<mark>0 010</mark>0  -  04<br>000<mark>0 011</mark>0  -  06<br>000<mark>0 100</mark>0  -  08<br>000<mark>0 101</mark>0  -  0A<br>000<mark>0 110</mark>0  -  0C<br>000<mark>0 111</mark>0  -  0E<br>000<mark>1 000</mark>0  -  10<br>000<mark>1 001</mark>0  -  12<br>000<mark>1 010</mark>0  -  14<br>000<mark>1 011</mark>0  -  16<br>000<mark>1 100</mark>0  -  18<br>000<mark>1 101</mark>0  -  1A<br>000<mark>1 110</mark>0  -  1C<br>000<mark>1 111</mark>0  -  1E)
```
