// c++ code of all the constructors

// code of constructor

#include<iostream>
using namespace std;

class A{
    private: int i=0;
    
    public:
        // Default constructors
    A(){
        cout << "This is the defaulf constructure,value of i is: " << i << endl << endl;
       }
       

       // Parameterise constructor
    A(int x, int y){
        cout << "This is constructure with parameters " << endl << endl;
        i = x+ y;
        cout << "Value of i now: " << i << endl;
      }

         
     // Copy constructors
     A(A &ob1) {
     i=ob1.i;
     cout << "Inside the copy constructor,value of i is same as ob1:" << i << endl << endl;
     }
};
 int main() {
    A obj;
   A ob1(5, 10);
}
