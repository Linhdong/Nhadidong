#include<conio.h>
#include<stdio.h>

void Pint_Binary (int n) 
{ 
  if(n==0)printf("0");
  else
  {
  stack S;
  Make_Null_Stack(S);
  while(n!0)
  {
  Push(n%2,S);
  n=n/2;
  }
  while(!Empty_Stack(S))
  { printf("%d",Top(S));
  Pop(S);
  }
  }
}
