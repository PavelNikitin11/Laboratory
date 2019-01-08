Lab1
Упражнение 1:
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

void main(void) {
	
	float x,y;
	
	printf("Write x",x);
	scanf("%g",&x);
	
	y = 16*pow(x,2);
	
	printf("%g Read",y);
}
Упражнение 2:
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

void main(void) {
	
	float x,y,z,a,b,u,r;
		
	printf("Write x",x);
	scanf("%g",&x);
	
	printf("Write y",y);
	scanf("%g",&y);
	
	printf("Write z",z);
	scanf("%g",&z);
	

    a = 9+(pow(x-y,2));
    b = (pow(a,1.0/3.0))/(pow(x,2)+ pow(y,2) + 2);
   
    u = (exp(fabs(x-y)))*(pow(tan(z),3));
    
	r = b-u;
    
	printf("%g read ",r); 
}
Lab2
Упражнение 1:
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include <locale.h>


void main(void) {
	setlocale(LC_ALL,"Russian");
		
	float R,B,S1,S2,p;
	
	p = 3.14;
	
	printf("Введите радиус R");
    scanf("%f",&R);
    
    printf("Введите сторону квадрата B");
    scanf("%f",&B);
    
    S1 = p*pow(R,2);
    S2 = pow(B,2);


    if (S1 > S2 ) printf("Можно вписать");
else  printf("Нельзя вписать");
}
Упражнение 2:
#include <stdio.h>
#include <stdlib.h>
#include <math.h>


void main() {

     
    float a,b,c;
	

printf("Enter a");
scanf("%f", &a);

printf("Enter b");
scanf("%f", &b);

printf("Enter c");
scanf("%f", &c);

if (a>0 && b>0 && c>0) printf("3");
  else if (a<0 && b>0 && c>0) printf("2");
  else if (a<0 && b<0 && c>0) printf("1");
  else if (a<0 && b<0 && c<0) printf("0");
  else if (a>0 && b>0 && c<0) printf("2");
  else if (a>0 && b<0 && c<0) printf("1");
  else if (a<0 && b>0 && c<0) printf("1");
}
Упражнение 3:
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include <locale.h>


void main(void) {
	setlocale(LC_ALL,"Russian");
	
	int n;
	printf("Введите номер месяца n");
    scanf("%d", &n);

     if (n==1 || n==2 || n==12) printf("Зима");
      else if (n>=3 && n<=5) printf("Весна");
       else if (n>=6 && n<=8) printf("Лето");
        else printf("Осень");
}
Lab3
Упражнение 1:
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include <locale.h>

void main(void) {
    setlocale(LC_ALL,"Ressian");
    
   float S,R,i,p;
    
    printf("read: ",S);
    scanf("%g",&S);
    
	R=S*2;
    i=1;
   
   while (S<=R){
	S=S+S*0.03;
	i++;
	}
	printf("read: %g",i);
}

Упражнение 2:
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include <locale.h>
void main(void) {
	setlocale(LC_ALL,"Russian");
	
	int  i,a,b,c,n;
	
	for (n=11;n<=31; n++){

		if(n%2!=0) {
		
			i =pow(n,2);
			a =(i/100);
			b = ((i%100)/10);
			c= ((i%100)%10);
	
			if((a<b) && (b<c)) printf("Числа:%d\n",i);
		}
	}
	
}
Lab4
Упражнение 1:
#include <stdio.h>
#include <stdlib.h>

/* run this program using the console pauser or add your own getch, system("pause") or input loop */

void main(void) {
	int t,i,k,N;
    int X[6]={2,4,3,6,5,8};
	
	for (i=0; i < 6/2; i++)
	{ t = X[i];X[i]= X[6-i-1]; X[6-i-1]= t;}
	
	for (k=0;k<6;k++)
	printf("%d ",X[k]);
	printf("\n");
	
}
Упражнение 2:
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main() {
	int n,s;
	n=0;
	s=0;
}

Lab5
Упражнение 1:
#include <stdio.h>
#include <stdlib.h>
/* run this program using the console pauser or add your own getch, system("pause") or input loop */

void main(void) {
	int i,j,k,n;
	int a[5][5];
	
	for(i=0;i<5;i++){
		for (j=0;j<5;j++)
			{
			a[i][j]=-5+rand()%20;
		}
		
	}
	printf("Matrix\n");
	
	for(i=0;i<5;i++){
		printf("\n");
		
		for(j=0;j<5;j++){
			
			printf("%d ",a[i][j]);//матрица
		}
	}  
Lab6

Упражнение 1:

#include <stdio.h>
#include <conio.h>
#include <stdlib.h>
#include <math.h>
#include <locale.h>
void main(void)
{
	int i,k,j,n;
	float a[n];
	k=0;
	scanf("%d",&n);
for (i=0;i<n;i++){
	a[i]=rand()%2;
	printf("%g ",a[i]);
	if(i%2!=0){
	k+=a[i];
	}
    
  }
  printf("%d ",k);
}
