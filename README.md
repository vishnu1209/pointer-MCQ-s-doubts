# pointer-MCQ-s-doubts
doubts
1.
#include <stdio.h>

int main()
{
    int i, *p = &i;
    scanf("%d", &i);
    foo(&p);
    printf("%d", *p);
    return 0;
}

void foo(int **p)
{
    int j;
    scanf("%d", &j);
    *p = &j;
    printf("%d ", **p);
}


2.
 #include <stdio.h>

int main()
{
    char *str = "IncludeHelp";

    scanf("%s", str);
    
    printf("%c",*&*str);
    return 0;
}

3.
#include <stdio.h>

char *strFun(void)
{
    char *str = "IncludeHelp";
    return str;
}

int main()
{
    char *x;
    x = strFun();
    printf("%s", x);
    return 0;
}

4.
#include <stdio.h>

int main()
{
    int i;
    scanf("%d", &i);
    int *j;
    int **k;
    j = &i;
    k = &j;
    k++;
    printf("%d ", k);
    return 0;
}
