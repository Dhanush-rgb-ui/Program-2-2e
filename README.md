#  Module-2 SEB
## AIM:
To write a C program for the pascal's triangle pattern:

<img width="162" height="157" alt="image" src="https://github.com/user-attachments/assets/0ca15556-863f-41db-9698-f98e704c5d0d" />

## Program:
```c
#include <stdio.h>
int main(){
    int row,i,j,num,space;
    scanf("%d",&row);
    for(i=0;i<row;i++){
        //spaces
        for(space=0;space<=row-i-2;space++){
            printf(" ");
        }
        //number
        num=1;
        for(j=0;j<=i;j++){
            printf("%d ",num);
            num=num*(i-j)/(j+1);
           
        }
        printf("\n");
    }
    return 0;
}
```
## Output:
<img width="441" height="480" alt="image" src="https://github.com/user-attachments/assets/e0fdeb8e-4180-4f21-9db9-21f9613d3ca9" />
