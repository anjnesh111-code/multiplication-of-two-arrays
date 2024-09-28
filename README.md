# multiplication-of-two-arrays
#include<iostream>
using namespace std;
int main() 
{
  int i , j ;
  cout<<"enter values of rows and columns : ";
  cin>>i;
  cin>>j;
  int arr[i][j],brr[i][j],c[i][j];
  cout<<"enter values of a : ";
  for(int a = 0; a < i; a++)
  {
    for(int b = 0; b < j; b++)
    {
      cin>> arr[a][b];
    }
  }  
  for(int a = 0; a < i; a++)
  {
    for(int b = 0; b < j; b++)
    {
      cout<<arr[a][b]<<" ";
    }
    cout<<endl;
  }  
  cout<<"enter values of b : ";
  for(int a = 0; a < i; a++)
  {
    for(int b = 0; b < j; b++)
    {
      cin>>brr[a][b];
    }
    cout<<endl;
  }   
   for(int a = 0; a < i; a++)
  {
    for(int b = 0; b < j; b++)
    {
      cout<<brr[a][b]<<" ";
    }
    cout<<endl;
  }   
   for(int a = 0; a < i; a++)
  {
    for(int b = 0; b < j; b++)
    {
      c[a][b]=0;
    }
    cout<<endl;
  }   
  for(int a=0;a<i;a++){
    for(int b=0;b<j;b++){
      for(int k=0;k<j;k++)
       c[a][b]+=arr[a][k]*brr[k][b];
    }  
    }
    for(int a = 0; a < i; a++)
  {
    for(int b = 0; b < j; b++)
    {
      cout<<c[a][b]<<" ";
    }
    cout<<endl;
  }

    return 0;
    }
