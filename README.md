# OPI
Problema//numeros

#include<iostream>
#include<math.h>

using namespace std;
int main()
{
    int base,expo = 0,modulo = 0;
    long long numero;
    cin>>base>>numero;
    for(int i = 1; i<=8; i++)
    {
        if(pow(base,i) == numero)
        {
            expo = i;
        }
    }
    modulo = expo;
    if(pow(base,expo)==numero)
    {
        cout<<"YES"<<endl;
        cout<<modulo - 1<<endl;
    }
    else
    {
        cout<<"NO"<<endl;
    }

    return (0);
}
