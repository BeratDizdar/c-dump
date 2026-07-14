```c
#include<stdio.h>
#include<ctype.h>
c,j;main(a,v)const char**v;{
    FILE*i=fopen(v[1],"rb"),*o=fopen(v[2],"w");
    for(;~(c=fgetc(i));j++){if(j%80==0)fprintf(o,"\n");
        fprintf(o,"%c",(isalnum(c)||ispunct(c))?c:'.');}
    fclose(i);fclose(o);
}
```
