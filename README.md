# C-code
#include <stdio.h>

//문제 1
/*
int main(void)
{
  printf("Hello\n\"World\"\n(%d 문제중 %d문제 정답 : %.1f%%)", 12, 7, 58.3);
  return 0;
}
*/

//문제 2
/*
int main(void)
{
  int n, a;
  printf("입력\n");
  scanf("%d %d", &n, &a);
  printf("\n출력\n");
  printf("%d ", n + a);
  printf("%d ", n - a);
  printf("%d ", n * a);
  printf("%d", n / a);
}
*/

//문제 3
/*
int main(void)
{
  int n, sum;
  do{
    printf("말해야 하는 수 : ");
    scanf("%d", &n);
  }while( !(0 < n &&n <2100000000) );

  while(n != 0)
  {
    int one;
    one = n % 10;
    if(one == 3 || one ==6 || one == 9)
    {
      sum++;
    }
    n /= 10;
  }
  printf("\n박수치는 횟수 : %d\n", sum);
  return 0;
}
*/
//문제 4
/*
int main(void)
{
  int n;
  printf("입력\n");
  scanf("%d", &n);
  printf("\n출력\n");
  for(int i; n >= 1; n--)
  {
    printf("%d ", n);
  }
  printf("Bang!\n");
  return 0;
}
*/
//문제 5

void rectangle(int n, int m);

int main(void)
{
  int n, m;
  printf("입력\n");
  scanf("%d %d", &n, &m);
  rectangle(n, m);
}

void rectangle(int n, int m)
{
  for(int i = 1; i <= n; i++)
  {
    printf("* ");
  }
  printf("\n");
  for(int i = 1; i <= (m - 2); i++)
  {
    printf("* ");
    for(int i = 1; i <= (n - 2); i++)
    {
      printf("  ");
    }
    printf("*\n");
  }
  for(int i = 1; i <= n; i++)
  {
    printf("* ");
  }
}
