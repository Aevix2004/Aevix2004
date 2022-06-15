#include <iostream>
using namespace std;
int main()
{
int i, ln, maxln;
const char*str="010011000111001";
for(i=1,ln=maxln=1;str[i];i++)
if (str[i]==str[i-1]){
ln++;
maxln=ln>maxln?ln:maxln;
}
else
ln=1;
cout<<maxln<<endl;
return 0;
}
