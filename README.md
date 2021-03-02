# 2021cce

hw

1
![1](https://user-images.githubusercontent.com/79676969/109654428-25d91e00-7b9d-11eb-8e87-6788a11f34a4.png)

```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	printf("%d=50*%d+5*%d+1*%d\n",n,n/50,n%50/5,n%5);
}
```
2
![2](https://user-images.githubusercontent.com/79676969/109654485-325d7680-7b9d-11eb-9ec6-16f584885cb3.png)

```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	printf("%d=50*%d+5*%d+1*%d\n",n,n/50,n%50/5,n%5);
}
```
3
![3](https://user-images.githubusercontent.com/79676969/109654523-3d180b80-7b9d-11eb-9309-a696a0817ca4.png)

```c
#include <stdio.h>
int main()
{
	int n,i,ans=0;
	for(int i=0;i<10;i++){
	scanf("%d",&n);
	if(n%3==0) ans++;
	}
	printf("%d\n",ans);
}

```
4
![4](https://user-images.githubusercontent.com/79676969/109654534-40ab9280-7b9d-11eb-9db5-85925217c921.png)

```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	
	if(n>=90) printf("A\n");
	else if(n<90&&n>=80) printf("B\n");
	else if(n<80&&n>=90) printf("C\n");
	else printf("F\n");
}
```
5
![5](https://user-images.githubusercontent.com/79676969/109654548-430dec80-7b9d-11eb-98a1-c2f5dbdf7ca4.png)

```c
#include <stdio.h>
int main()
{
	int n,m,temp;
	scanf("%d%d",&n,&m);
	if(m>n) temp=n;
	else temp=m;
	int ans;
	for(int i=1;i<=temp;i++){
		if(n%i==0&&m%i==0) ans=i;
	}
	printf("%d %d\n",n/ans,m/ans);
}
```
