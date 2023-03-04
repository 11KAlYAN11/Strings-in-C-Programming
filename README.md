# Strings-in-C-Programming

Date :13/05/2021

strings in c programming
BASIC STRING OPERATIONS 

1...)
#include<stdio.h>  
#include <string.h>    
int main()
{
    char ch1[30] = "asam kalyan reddy";
    char ch2[15] = {'a','s','a','m','k','a','l','y','a','n','\0'};
    char ch3[30];
    if(strcmp(ch1,ch2)==0)
    {
        printf("both are Equal \n");
    }
    else
        printf("both are not equal\n");
    strcat(ch1,ch2);
    printf("cancaatenation string is : %s\n",ch1);
    strcpy(ch2,ch1);
    printf("copied string is %s\n",ch2);
    printf("Lenghth of string 1 and string 2 is : %d \t %d\n",strlen(ch1),strlen(ch2));
    printf("\n\nReverseing the strings As : %s \n %s\n\n",strrev(ch1),strrev(ch2));//maybe strrev not working properly bcz previous operations is there so try it seperately
    printf("string in lower case : %s\t %s\n",strlwr(ch1), strlwr(ch2));
    printf("string in upper case : %s \t %s\n",strupr(ch1),strupr(ch2));


}

o/p:
both are not equal
cancaatenation string is : asam kalyan reddyasamkalyan
copied string is asam kalyan reddyasamkalyan
Lenghth of string 1 and string 2 is : 12         27


Reverseing the strings As : asam kalyan
 naylakmasaydderasam kalyan

string in lower case : asam kalyan       naylakmasaydderasam kalyan 
string in upper case : ASAM KALYAN       NAYLAKMASAYDDERASAM KALYAN

2..)
#include<stdio.h>  
#include <string.h>    
int main()
{
    char ch1[30] = "asam kalyan reddy";
    char ch2[15] = {'a','s','a','m','k','a','l','y','a','n','\0'};
    printf("\n\nReverseing the strings As : %s \n %s\n\n",strrev(ch1),strrev(ch2));
    
}
o/p:
Reverseing the strings As : ydder naylak masa 
 naylakmasa


3...)

C MATH FUNCTIONS'

#include<stdio.h>  
#include<math.h>    
int main()
{
    printf("%f\n",ceil(3.6));
    printf("%f\n",ceil(3.2));
    printf("%f\n",floor(3.9));
    printf("%f\n",floor(3.2));
    printf("%f\n",sqrt(16));
    printf("%f\n",sqrt(64));
    printf("%f\n",pow(2,4));
    printf("%f\n",pow(8,2));
    printf("%d\n",abs(-12));
    printf("%d\n",abs(-234));
}
   

o/p:
4.000000
4.000000
3.000000
3.000000
4.000000
8.000000
16.000000
64.000000
12
234

4...)

printing time and date:
#include<stdio.h>  
 int main(){    
  printf("File : %s\n",__FILE__);
  printf("DAte : %s\n",__DATE__);
  printf("Time :%s\n",__TIME__);
  printf("Line : %s\n",__LINE__);
  printf("STDC : %d\n",__STDC__);
 }    

o/p:
File : kalyan1.c
DAte : May 14 2021
Time :14:20:48
Line :



