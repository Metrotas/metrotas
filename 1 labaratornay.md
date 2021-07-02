### Hi there 👋

Лабараторная работа 1
1) #include <iostream>
#include <iomanip>
using namespace std;
int main()
{
    const int M=10;
    int a[M];
    for (int i=0; i<M;i++)
    {
        cout<<"Vvedite element ["<<i<<"]:";
        cin>>a[i];
    }
    for (int i=0; i<M; i++)
    {
        if (a[i]%2==0)
        a[i]=0;
        cout<<&apos; &apos;<<a[i]<<&apos; &apos;;
    }
}



2#include <iostream>
#include <stdio.h>
#include <cstring>
using namespace std;
int main ()                              
{
    string s;                                        
    int n, m;                                              
    do {
        cout << "Введите символ: ";
            cin >> n;
            if(!cin) 
        {
       cout << "Ошибка, введите символ: \n";
       cin.clear();
       while (cin.get() != &apos;\n&apos;);
            }
                else 
                break;
    } while (true);
    cout << "Введите строчку: " << endl;
    do {
        cin >> s;
        if (s.size() < 1) {                             
            cout << "Ошибка, введите строчку: " << endl;
            s.clear();
        }
        else
            break;
    } while (true);
    m = s.find(n);                                      
    if (m != -1) cout << "Введенный символ не найден" << endl;
    else {cout << "Введенный символ находится на: " << m+3 << " позиции" << endl;}
    }



3) #include <iostream>
#include <iomanip>
 
using namespace std;
 
int main()
{
    int a[3][3]; float d;
    cout << "Enter matrix:" << endl;
    for (int i = 0; i < 3; i++)                
    {
        for (int j = 0; j < 3; j++)
            cin >> a[i][j];
        cout << "Enter next string" << endl;
    }
    cout << endl << endl << "Your matrix:" << endl;  
    for (int i = 0; i < 3; i++)               
    {
        for (int j = 0; j < 3; j++)
            cout << setw(5) << a[i][j];
        cout << endl << endl;;
    }
    d = a[0][0] * a[1][1] * a[2][2] + a[0][1] * a[1][2] * a[2][0] + a[0][2] * a[1][0] * a[2][1] - a[0][2] * a[1][1] * a[2][0] - a[0][0] * a[1][2] * a[2][1] - a[0][1] * a[1][0] * a[2][2];  
    cout << setprecision(4) << d;
    return 0;
}

