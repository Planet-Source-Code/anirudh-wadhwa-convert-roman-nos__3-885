<div align="center">

## Convert\_Roman\_Nos\.


</div>

### Description

THIS IS THE "FASTEST" ALGORITHM FOR CONVERSION OF ROMAN NUMERALS INTO NUMBERS.IT WILL CONVERT ALL ROMAN NUMERALS INTO NUMBERS IN RECORD TIME.IF ANY ONE KNOWS ANY FASTER METHOD PLEASE LET ME KNOW.
 
### More Info
 
THIS PROGRAM WILL CONVERT ROMAN NUMERALS INTO NUMBERS REGARDLESS OF THEIR CASE.XXIV = xxiv = 24


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Anirudh Wadhwa](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/anirudh-wadhwa.md)
**Level**          |Intermediate
**User Rating**    |5.0 (15 globes from 3 users)
**Compatibility**  |C, C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+, UNIX C\+\+
**Category**       |[Algorithms](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/algorithms__3-29.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/anirudh-wadhwa-convert-roman-nos__3-885/archive/master.zip)





### Source Code

```
#include <iostream.h>
#include <string.h>
#include <conio.h>
#include <stdlib.h>
//For Any Queries,MailMe themask99@yahoo.com
void main()
{
char a[15];
cout<<"Enter The Roman Number :";
cin>>a;
for(int x=0,p=0,flag=0,rom=0,int i=strlen(a)-1;i>=0;i--)
	{
	if (a[i]=='i' || a[i]=='I') x=1;
    if (a[i]=='v' || a[i]=='V') x=5;
	if (a[i]=='x' || a[i]=='X') x=10;
	if (a[i]=='l' || a[i]=='L') x=50;
	if (a[i]=='c' || a[i]=='C') x=100;
	if (a[i]=='d' || a[i]=='D') x=500;
	if (a[i]=='m' || a[i]=='M') x=1000;
	if (x<p) flag = -1;
	else flag = 1;
	rom= rom + (x*flag);
	p=x;	//storing the previous value in x
	}
cout<<"Numerical value is : "<<rom;
getch();
}
```

