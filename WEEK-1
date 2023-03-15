Q-1: 

//Linear Search//
#include<stdio.h>
void main()
{
    int a[20],n,i,k,c=0,f=0;
    printf("Enetr limit: ");
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    printf("Enter the key:");
    scanf("%d",&k);
    for(i=0;i<n;i++)
    {
        if(a[i]==k)
        {
            f=1;
            c++;
        }
        else
        c++;
    }
    if(f!=0)
    {
        printf("Key found\n");
        printf("Comparison=%d",c);
    }
    else
    printf("Key not found");
}

INPUT:
Enter limit:5
13 17 11 4 20
Enter key:11
OUTPUT:
Key found
Comparison=5

Q-2:
//Binary Search//
#include <stdio.h>
int main()
{
  int i,l,h,mid,n,key,a[10];
  printf("Enter limit:");
  scanf("%d",&n);
  printf("Enter elements:");
  for(i=0;i<n;i++)
  {
   scanf("%d",&a[i]);
  }
  printf("Enter the key:");
  scanf("%d", &key);
  l = 0;
  h = n - 1;
  mid = (l+h)/2;
  while (l <= h) 
  {
    if(a[mid] < key)
      l = mid + 1;
    else if (a[mid] == key) 
    {
      printf("%d found at location %d", key, mid+1);
      break;
    }
    else
      h = mid - 1;
    mid = (l + h)/2;
  }
  if(l > h)
  printf("Not found! %d isn't present in the list", key);
  return 0;
}

INPUT:
Enter limit:5
Enter elements:11 19 22 23 24
Enter the key:23
OUTPUT:
23 found at location 4


Q-3:
//Jump Search//
#include<iostream>
#include<math.h>
using namespace std;
int jumpsearch(int a[],int c,int n)
{
    int l=0,h=sqrt(c),i;
    while(a[h]<=n && h<c)
    {
        l=h;
        h+= sqrt(c);
        if(h > c-1)
        {
            h=c;
        }
    }
    for(i=l;i<h;i++)
    {
        if(a[i]==n)
        {
            return i;
        }
    }
    return l;
}
int main()
{
    int a[20],b,c,i,j,n;
    cout<<"Input no of test cases:";
    cin>>b;
    for(i=0;i<b;i++)
    {
        cout<<"Enter limit:";
        cin>>c;
        cout<<"Enter elements:";
        for(j=0;j<c;j++)
        {
            cin>>a[j];
        }
        cout<<"Enter element to be searched:";
        cin>>n;
        int res=jumpsearch(a,c,n);
        if(res==c)
        cout<<"Not present";
        else if(a[res]==n)
        cout<<"Present at index= "<<res<<endl;
        else
        cout<<"Not present";
    }
    return 0;
}

INPUT:
Enter the number of test cases:1
Enter limit:5
Enter elements:1 2 3 4 5
Enter the element to be searched:3
OUTPUT:
Present at index= 2
