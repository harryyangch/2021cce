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
-------------------------------------------------------------------------------------------------------------
1
```c
#include <stdio.h>
int a[1000];
int main()
{
	int N=0;
	for(int i=0;i<1000;i++){
		scanf("%d",&a[i]);
		if(a[i]==0){
			N=i;
			break;
		}
	}
	for(int i=N-1;i>=0;i--){
		printf("%d ",a[i]);
	}
	printf("\n");
}
```
3
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	int ans=0;
	for(int i=1;i<=n;i++){
		ans=ans+i*(i-1);
	}
	printf("%d\n",ans);
}
```
4
```c
#include <stdio.h>
int main()
{
	printf("Enter two numbers:  ");
	int n,m;
	scanf("%d%d",&n,&m);
	if(n==m) printf("It is a square ");
	else printf("It is not a square ");
}
```
5
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	
	int ans=0;
	if(n/1000==1) ans+=8;
	if(n%1000/100==1) ans+=4;
	if(n%100/10==1) ans+=2;  
	if(n%10==1) ans+=1;
	
	printf("%d\n",ans);
}
```
6
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	
	int ans=0;
	if(n/1000==1) ans+=8;
	if(n%1000/100==1) ans+=4;
	if(n%100/10==1) ans+=2;  
	if(n%10==1) ans+=1;
	
	printf("%d\n",ans);
}
```
------------------------------------------------------------------------------------------------------------------
1.
![week04-1](https://user-images.githubusercontent.com/79676969/112484395-db6e4a00-8db4-11eb-9100-f1458c902de6.png)
```c
#include <stdio.h>
int main()
{
	int a[5]={0,10,20,30,40};
	int *p=&a[2];
	*p=222;
	
	p=p+2;
	*p=666;
}
```
2.
![week03-2](https://user-images.githubusercontent.com/79676969/111619700-d9d6dc00-8820-11eb-94b1-a3dffd41f9af.png)
```c
#include <stdio.h>
int a[5]={0,10,20,30,40};
void printAll(){
	for(int i=0;i<5;i++0 printf"%d",a[i]);
	printf("\n");
}
int main()
{
		printAll();
	int *p=&a[2];
	*p=222;
		printAll();
	p=p+2;
	*p=666;
		printAll();
	p--;
	*p=555;
		printAll();
}
```
3.
![week03-3](https://user-images.githubusercontent.com/79676969/111619765-e8bd8e80-8820-11eb-8854-27fb24b71d4a.png)

```c
#include <stdio.h>
int a[5]={0,10,20,30,40};
void printAll(){
	for(int i=0;i<5;i++0 printf"%d",a[i]);
	printf("\n");
}
int main()
{
		printAll();
	int *p=&a[2];
	*p=222;
		printAll();
		printf("p心裡小紙條記的值是:%d\n",p);
	p=p+2;
	*p=666;
		printAll();
		printf("p心裡小紙條記的值是:%d\n",p);
	p--;
	*p=555;
		printAll();
		printf("p心裡小紙條記的值是:%d\n",p);
}
```
4.
![week03-4](https://user-images.githubusercontent.com/79676969/111619819-f5da7d80-8820-11eb-98c8-ff8bb4d76e43.png)
```c
#include <stdio.h>
#include <stdiib.h>
int a[10];
int main()
{
	int b[10];
	int *p=(int*) malloc(sizeof(int)*10);

	return 0;
}

```
----------------------------------------------------------------------------------------
#week 04
1.       ![Uploading week04-1.png…]()

#include <stdio.h>
struct POINT{
    float x,y;
};
int main(){
    struct POINT a={4.1,3.2};
    printf("%f%f\n",a.x,a.y);

    return 0;
}
2.![week04-2](https://user-images.githubusercontent.com/79676969/112483889-69960080-8db4-11eb-85d1-04859f75b6ba.png)
```c
#include <stdio.h>
struct POINT{
    float x,y;
};
int main(){
    struct POINT a={4.1,3.2};
    printf("%f%f\n",a.x,a.y);

  
}
```
3.![week04-3](https://user-images.githubusercontent.com/79676969/112484054-90eccd80-8db4-11eb-8dd7-ccda07d29b14.png)
```c
#include <stdio.h>
struct POINT{
    float x,y;
};
int main(){
    struct POINT a={4.1,3.2};
    printf("%f%f\n",a.x,a.y);

    return 0;
}
```

4.![week04-4](https://user-images.githubusercontent.com/79676969/111726234-7d68d080-88a3-11eb-9dc7-84a92a0d0f4d.png)
```c
#include <stdio.h>
struct DATA{
    int x,y;
}a[3];
struct DATA b={100,200};

int main(){
    for(int i=0;i<3;i++){
        printf("a[%d]:%d %d\n",i,a[i].x,a[i].y);
    }
    printf("b: %d %d\n",b.x,b.y);

    struct DATA c;
    printf("c: %d %d 像亂碼\n",c.x,c.y);
    c=b;

    printf("c: %d %d\n",c.x,c.y);
}
```
5.![week04-5](https://user-images.githubusercontent.com/79676969/111728796-93c55b00-88a8-11eb-8e4d-5c6dd9fb0db5.png)
```c
#include <stdio.h>
struct POINT{
    float x,y,z;
};

struct POINT point[5]={{0,0,0},{1,0,0},{0,1,0},{0,0,1},{1,1,1}};

int main()
{
   struct POINT*p=&point[0];
   printf("%.2f %.2f %.2f\n",p->x,p->y,p->z);

   p++;
   printf("%.2f %.2f %.2f\n",p->x,p->y,p->z);

   p++;
   printf("%.2f %.2f %.2f\n",p->x,p->y,p->z);
}
```
week 7


![week07-2](https://user-images.githubusercontent.com/79676969/114888180-95e4f000-9e3b-11eb-9806-75e10100ce3c.png)

![week07-3](https://user-images.githubusercontent.com/79676969/114888216-9b423a80-9e3b-11eb-9217-a19055316948.png)


----------------------------------------------------------------------------------------
week8


![week08-7](https://user-images.githubusercontent.com/79676969/115737033-5c256380-a3be-11eb-8159-cca9040f25c0.png)


----------------------------------------------------------------------------------------
week10

1.
```c
#include <stdio.h>
int main()
{
	int T;
	scanf("%d\n\n",&T);
	
	for(int t=0;t<T;t++){
		int N=0;
		while(gets(line)!=NULL){
			if(strcmp(line,"")==0) break;
			
			printf("%s\n",line);
		}
		printf("====分隔線=====\n");
	}
}
```
![week10-1](https://user-images.githubusercontent.com/79676969/116642805-41488580-a9a2-11eb-8b9d-ac0f35d92435.png)

2.
```c
#include <stdio.h>
int main()
{
	int T;
	scanf("%d\n\n",&T);
	
	for(int t=0;t<T;t++){
		int N=0;
		while(gets(line)!=NULL){
			if(strcmp(line,"")==0) break;
			
			//printf("%s\n",line);
			N++;
		}
		printf("有幾棵樹?%d\n",N);
		printf("====分隔線=====\n");
	}
}
```
![week10-2](https://user-images.githubusercontent.com/79676969/116643552-e152de80-a9a3-11eb-9f45-12d9df7a6e9d.png)



