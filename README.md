# Project1
#include<stdio.h>
#include<conio.h>
void main()
{
    int i,j,count=0,count1=0,m=0;
    char s[10];
  char str[20];
  printf("enter any string:\n");
  scanf("%s",&str);
  printf("enter substring to which wil be chacked:\n");
  scanf("%s",&s);
  m=strlen(s);
  for(i=0;str[i]!='\0';)
  {
      count=0;
      for(j=0;s[j]!='\0';j++)
      {
          if(str[i++]==s[j])
          count++;
          else
          break;
      }
      if(count==m)
      count1++;
  }
  printf("%d",count1);
}


