# GCD program in c language.
#include <stdio.h>
int a, b, c ,g;
int gcd(){
    printf("working with %d \n",a);
    if (b%a ==0 && c%a ==0)  
    g = a;
    else {
        a--;
        return gcd();
    }
}
int main()
{
    int temp;
    printf("give 3 values \n");
    scanf("%d %d %d", &a, &b ,&c);
    
    if (b<a){
        temp = a;
        a = b;
        b = temp;
    }
    g = gcd();
    printf("the GCD of numbers %d %d %d is %d \n",a, b, c, g);
}
