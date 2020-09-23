<div align="center">

## A simple strings sorting


</div>

### Description

This code will make you understand simple by accepting 4 strings and sorting it through Bubble sort i trust this u help for C and C++ Beginner.
 
### More Info
 
Ask to enter 4 strings

User should be aware of Arrays, boolean,for loops.

returns sorting strings

Not much its only like beginiing of C and C++ Programer


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Tahseen](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/tahseen.md)
**Level**          |Beginner
**User Rating**    |4.2 (21 globes from 5 users)
**Compatibility**  |C, C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+
**Category**       |[Sorting](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/sorting__3-24.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/tahseen-a-simple-strings-sorting__3-3714/archive/master.zip)

### API Declarations

```
#include <iostream.h>
#include <string.h>
```


### Source Code

```
#define ELEMENT 4
#define LENGTH 20
void getdata(char str[ELEMENT][LENGTH]);
void show(char str[ELEMENT][LENGTH]);
void sort(char str[ELEMENT][LENGTH]);
void main()
{
  char str[ELEMENT][LENGTH];
  cout<<"Find the sortin of string\n";
  getdata(str);
  sort(str);
  show(str);
}
void getdata(char str[ELEMENT][LENGTH])
{
  int loop;
  for(loop=0;loop<ELEMENT;loop++)
  {
  	cin.getline(str[loop],LENGTH);
  }
}
void sort(char str[ELEMENT][LENGTH])
{
  char temp[LENGTH];
  int loop;
  bool flag;
  do
  {
   flag=false;
   for(loop=0;loop<ELEMENT;loop++)
   {
   	if(strcmp(str[loop],str[loop+1])>0)
     {
   	flag=false;
     strcpy(temp,str[loop]);
     strcpy(str[loop],str[loop+1]);
     strcpy(str[loop+1],temp);
     flag=false;
     }
   }
  }while(flag!=false);
}
void show(char str[ELEMENT][LENGTH])
{
  int loop;
  cout<<endl;
  for(loop=0;loop<ELEMENT;loop++)
  {
  	cout<<str[loop]<<endl;
  }
}
```

