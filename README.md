# c-problems
extracting numbers from string
#include<stdio.h>
//#include<conio.h>
int main()
{
  char s[]="hello123 t254his is 234 786s";
  char *p=s;
  while(*p != NULL)
  {
    if(isdigit(*p) && isdigit(*(p+1)) && isdigit(*(p+2)))
    {
      printf("%c%c%c\n",*p,*(p+1),*(p+2));
      p=p+3;
    }
    p++;
  }
  return 0;
}
