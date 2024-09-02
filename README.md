# experiment-10
Aim:
To study and implement Pointer Operations (call by value and call by reference)

Theory:
There are two ways to call a variable to a function for various operations.

 call by value 
1)A method of passing arguments to a function where the actual value is passed.
2)Does not affect the original variable.
3)More memory is used because a copy of the actual value is made.
4)Used when the function does not need to modify the original data.

call by Call by Reference
1)A method of passing arguments where the address of the variable is passed.
2)	Does affect the original variable.
3)Less memory is used because only the address is passed.
4)Used when the function needs to modify the original data or when passing large objects.

code:
a.
```

#include <iostream>'
using namespace std;

//call by value
int a,b;
void swap (int a, int b)
{
    int sw;
    sw = a;
    a = b;
    b = sw;
    cout<<"Swapped Values: "<<endl;
    cout<<"a: "<<a<<endl;
    cout<<"b: "<<b<<endl;
}

int main()
{
    int a,b;
    cout<<"Using call by value: "<<endl;
    cout<<"Enter a number: ";
    cin>>a;
    cout<<"Enter another number: ";
    cin>>b;
    cout<<"User Values: "<<endl;
    cout<<"a: "<<a<<endl;
    cout<<"b: "<<b<<endl;
    swap(a,b);
    
}

b.
'''cpp
#include <iostream>
using namespace std;

//call by value
int a,b;
int *pa, *pb;
void swapr (int *pa, int *pb)
{
    int *psw;
    int sw;
    psw = &sw;
    *psw = *pa;
    *pa = *pb;
    *pb = *psw;
    cout<<"Swapped Values: "<<endl;
    cout<<"a: "<<*pa<<endl;
    cout<<"b: "<<*pb<<endl;
}

int main()
{
    int a,b;
    int *pa, *pb;
    cout<<"Using call by value: "<<endl;
    cout<<"Enter a number: ";
    cin>>a;
    pa = &a;
    cout<<"Enter another number: ";
    cin>>b;
    pb = &b;
    cout<<"User Values: "<<endl;
    cout<<"a: "<<a<<endl;
    cout<<"b: "<<b<<endl;
    swapr(pa,pb);
    
}
```
outpute ![image](https://github.com/user-attachments/assets/5744569d-a3b9-4639-ab43-d07796558456)
![image](https://github.com/user-attachments/assets/21020783-9865-4b34-b0c7-e87d287247ca)




Conclusion:
→ We learnt about call by value and call by reference in C++.

→ We learnt the use case of each in C++.

