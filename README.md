#include<stdio.h>
//#include<conio.h>
int main()
{
  char s[100]="sdklgghf12";
  //scanf("%s",s);
  int count=0;
  char *p=s;
  while(*(p) != NULL)
  {
    if(!isdigit(*(p-1)) && isdigit(*p) && isdigit(*(p+1)) && isdigit(*(p+2)) && !isdigit(*(p+3)))
    {
      printf("%c%c%c\n",*p,*(p+1),*(p+2));
      p=p+3;
      count++;
    }
    p++;
    
  }
  if(count==0)
    printf("-1");
  
  return 0;
}

