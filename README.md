# 2020-cce
```
#include <stdio.h>
int main()
{
	int a, b, c;
	scanf("%d%d", &a, &b);
	int x=a, y=b;
	while(b!=0)
	{
		c=b;
		b=a%b;
		a=c;
	}
	printf("%d %d\n", x/a, y/a);
}
```
```
#include <stdio.h>
int main()
{
	int a[1000], n=0;
	for(int i=1;i<=1000;i++)
	{
		scanf("%d", &a[i]);
		n++;
		if(a[i]==0) break;
	}
	for(int j=n-1;j>=1;j--)
	{
		printf("%d ", a[j]);
	}
	printf("\n");
}
```
```
#include <stdio.h>
int MYPOWER(int a, int b)
{
	int ans=1;
	for(int i=1;i<=b;i++)
	{
	ans*=a;
	}
	return ans;
}
int main(void)
{
	int a,b;
	scanf("%d%d",&a,&b);
	printf("[%d]",MYPOWER(a,b));
	return 0;
}
```
```
#include <stdio.h>
int main()
{
	int a, ans=0;
	scanf("%d", &a);
	for(int i=a;i>=1;i--)
	{
		ans=ans+i*(i-1);
	}
	printf("%d\n", ans);
}
```
```
#include <stdio.h>
int main()
{
	int a, b, c, d;
	scanf("%d", &a);
	b=a/50;
	c=(a-(50*b))/5;
	d=(a-(50*b+5*c));
	printf("%d=50*%d+5*%d+1*%d\n", a, b, c, d);
}
```
```
#include <stdio.h>
int main()
{
	int a, b;
	b=1;
	scanf("%d", &a);
	for(int i=1;i<a;i++)
	if(a%i==0)
	{
		b++;
	}
	printf("%d\n", b);
}
```
```
#include <stdio.h>
int main()
{
	int a[11], n=0;
	for(int i=1;i<11;i++)
	{
		scanf("%d", &a[i]);
		if(a[i]%3==0) n=n+1; 
	}
	printf("%d\n", n);
}
```
```
#include <stdio.h>
int main()
{
	int a;
	scanf("%d", &a);
	if(a>=90)
	printf("A\n");
	else if(a<90 && a>=80)
	printf("B\n");
	else if(a<80 && a>=60)
	printf("C\n");
	else
	printf("F\n");
}
```
