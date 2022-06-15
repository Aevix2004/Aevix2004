#include <stdio.h>
#include <iostream>
#include <time.h>
using namespace std;
int main()
{
    int m,n,i,j;
    cout<<"vvedite chislo strok"<<endl;
    cin>>n;
    cout<<"vvedite chislo stolbcov"<<endl;
    cin>>m;
    int mas[n][m],sum=0;
srand(time(NULL));
for (int i = 0; i< n; i++){
for (int j = 0; j< m; j++){ 
mas[i][j] =1 + rand()%10;}}
cout<<"Displaying array elements:"<<endl;
for (int i = 0; i< n; i++) {
for (int j = 0; j< m; j++){
cout<<mas[i][j];
cout<<endl;
}}
for (int i = 0; i< n; i++) {
for (int j = 0; j< m; j++){
if(i==j) sum+=mas[i][j];
}}
cout<<"Sum of it "<<sum<<endl;
system ("pause");
return 0;
}
