# smallest-and-second-smallest

#include <stdio.h>

int main()
{
    int a[]={1,2,3,4,5};
    int n=5;
    int small=a[1];
    int secondsmall=a[0];
    
    for (int i=0;i<n;i++){
        if(a[i]<small){
            secondsmall=small;
            
            small=a[i];
        }
        else if (a[i]<secondsmall && a[i] > small){
            secondsmall=a[i];
        }
    }
    printf("small numbers=%d \n",small);
    printf("secondsmall numbers=%d \n",secondsmall);
}
