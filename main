#include <iostream>
#include <conio.h>
#include <cstdlib>
#define MAX

using namespace std;

typedef struct
{
    int ukrn;
    int top;
    int data[MAX];
}STACK;

STACK tumpuk;

void Ukuran()
{
    cout<<" Input ukuran STACK : ";cin>>tumpuk.ukrn;
    tumpuk.data[tumpuk.ukrn];
}

void Create()
{
    tumpuk.top=-1;
}

int IsEmpty()
{
    if(tumpuk.top==-1)
        return 1;
    else
        return 0;
}
int IsFull()
{
    if(tumpuk.top==tumpuk.ukrn-1)
        return 1;
    else
        return 0;
}

void Push(int isi)
{
    if(IsFull() == 0)
    {
        tumpuk.top++;
        tumpuk.data[tumpuk.top] = isi;
        cout<<" Data ("<<tumpuk.data[tumpuk.top]<<") sudah dimasukkan"<<endl;
    }

    else
    {
        cout<<" STACK sudah penuh, data tidak bisa dimasukkan"<<endl;
    }

}

void Pop()
{
    if(IsEmpty() == 0)
    {
        cout<<" Data ("<<tumpuk.data[tumpuk.top]<<") sudah dikeluarkan"<<endl;
    }

    else
    {
        cout<<" STACK kosong";

    }
    tumpuk.top--;
}

void View()
{
    if(IsEmpty() == 0)
    {
        for(int i=tumpuk.top; i>=0; i--)
        {
            cout<<" Data ke-"<<i+1<<" = "<<tumpuk.data[i]<<endl;
        }
    }

    else
    {
        cout<<" STACK kosong"<<endl;
    }

}

void Clear()
{
    tumpuk.top=-1;
    cout<<" STACK sudah dikosongkan"<<endl;
}

int main()
{
    int pilih,isi;
    Create();

    do
    {
        system("cls");
        cout<<"-------------------------------------------------"<<endl;
        cout<<"                  PROGRAM STACK                  "<<endl;
        cout<<"-------------------------------------------------"<<endl;
        cout<<" 1. STACK Size"<<endl;
        cout<<" 2. Push"<<endl;
        cout<<" 3. Pop"<<endl;
        cout<<" 4. View"<<endl;
        cout<<" 5. Clear"<<endl;
        cout<<" 6. Exit"<<endl;
        cout<<"-------------------------------------------------"<<endl;
        cout<<" Pilih Menu : ";cin>>pilih;

        while(pilih >6)
        {
            cout<<" Pilih Angka 1-5";
            break;
        }

        switch(pilih)
        {
            case 1:
                cout<<"-------------------------------------------------"<<endl;
                Ukuran();
                break;
            case 2:
                cout<<"-------------------------------------------------"<<endl;
                cout<<" Masukkan data : ";cin>>isi;
                Push(isi);
                break;
            case 3:
                cout<<"-------------------------------------------------"<<endl;
                Pop();
                break;
            case 4:
                cout<<"-------------------------------------------------"<<endl;
                View();
                break;
            case 5:
                cout<<"-------------------------------------------------"<<endl;
                Clear();
                break;
            case 6:
                cout<<"-------------------------------------------------"<<endl;
                cout<<" Program Selesai, Terimakasih"<<endl;
        }
        cout<<"-------------------------------------------------"<<endl;
        cout<<" Tekan ENTER untuk lanjut"<<endl;
        getch();
    }
    while(pilih!=6);
    cout<<"-------------------------------------------------"<<endl;
    cout<<" Tekan ENTER untuk keluar";
    getch();
}
