#include <stdio.h>

int main() {
    int n, i; 

    printf("Enter the size of the array: ");
    scanf("%d", &n); 

    int arr[n];  
    printf("Enter elements of the array:\n");
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);  

    printf("Array elements are:\n");
    for (i = 0; i < n; i++) {
        printf("%d ", arr[i]);  
    }

    return 0;
}



#include <stdio.h>

void insert(int arr[], int *n, int pos, int val) {
  
   
    for (int i = *n; i > pos; i--)
        arr[i] = arr[i - 1];

    arr[pos] = val;

    (*n)++;
}

int main() {
    int arr[7] = {10, 20, 30, 40, 50};
    int n = 5;
    int pos = 3;
    int val = 25;

    insert(arr, &n, pos, val);

    for (int i = 0; i < n; i++)
        printf("%d ", arr[i]);
    return 0;
}


 #include <stdio.h>
    void main()
    {
 
        int i, j, a, n, number[30];
        printf("Enter the value of N \n");
        scanf("%d", &n);
 
        printf("Enter the numbers \n");
        for (i = 0; i < n; ++i)
            scanf("%d", &number[i]);
 
        for (i = 0; i < n; ++i) 
        {
 
            for (j = i + 1; j < n; ++j)
            {
 
                if (number[i] > number[j]) 
                {
 
                    a =  number[i];
                    number[i] = number[j];
                    number[j] = a;
 
                }
 
            }
  }
 
        printf("The numbers arranged in ascending order are given below \n");
        for (i = 0; i < n; ++i)
            printf("%d\n", number[i]);
 
    }


#include<stdio.h>
int main()
{
    int arr[9]={5,24,36,48,52,64,88,96,100};
    int n=9,l,h,key,mid;
    l=0,h=n-1,key=88;
    while(l<=h)
    {
        mid=(l+h)/2;
        if(mid==key)
        {
            printf("Found");
        }
        else if(mid<key){
            l=mid+1;
        }
        else{
            h=mid-1;
        }
    }
   printf("%d",mid);
    
}



    
