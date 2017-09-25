# TEMPO
#include <string>
#include <ctime>
#include <cstdlib>
#include <iostream>
#include <windows.h>

using namespace std;

int main()


{

    int hr;
    int minu;
    int seg;
    int x;
    int tim;
    int c;
    int ms;
string tiempo;




    cout<<"introduce el tiempo con el formato HH:MM:SS";
    cin>>tiempo;



    string hora = tiempo.substr (0,2);
    string minuto = tiempo.substr (3,2);
    string segundo = tiempo.substr (6,2);

    hr = atoi (hora.c_str());
    minu = atoi (minuto.c_str());
    seg = atoi (segundo.c_str());
    tim = atoi (tiempo.c_str());



do
    {
        for(seg=0;seg>60;seg--){
            Sleep(1000);
            cout<<hr<<":"<<minu<<":"<<seg<<endl;
        }

    if(minu==0){

            if(hr==0 && seg==0){


            cout<<hr<<":"<<minu<<":"<<seg<<endl;
    hr--;
    minu=60;
    seg=60;

            }

    }

    else{
        Sleep(1000);
        minu--;
        seg=60;

        cout<<hr<<":"<<minu<<":"<<seg<<endl;

    }

    }while(x==1);




    }
