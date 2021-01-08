# print-fibonacci
Write a C++ code that will print  “*” based on Fibonacci series.


#include <iostream>
using namespace std;

int main(){

    int R , a = 0 , b = 1, temp , nextTerm;
    cout << "Enter the range of Fibonacci: ";
    cin >> R;
    for(int i = 0; i<=R; i++){
        if(i==0){
            cout << endl;
            continue;
        }
        if(i==1){
            cout << "*" << endl;
            continue;
        }
        if(i==2){
            continue;
        }

        nextTerm = a + b;
        a = b;
        b = nextTerm;

        for(int j = 1; j <= b; j++){
            cout << "* ";
        }
        cout << endl;


    }

    return 0;
}
