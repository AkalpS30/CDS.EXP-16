# CDS.EXP-16
## Aim:
**To study and implement Exception Handling in C++.**

## Software:
`Microsoft VSCode`

## Theory:
<ul>
    <li>In C++ exceptions are runtime anomalies or abnormal conditions that a program encounters durig its execution. </li>
    <li>The process of handling these exceptions is known as exception handling. </li> 
    <li>Using the exception handling mechanism, the control from one part of the program where the exception occurred can be transferred to another part of the 
   code.</li>
    <li>It can be done using three keywords: <ol>
        <li>try - The try keyword represents a block of code that may throw an exception placed inside the try block. It’s followed by one or more catch blocks. If an exception occurs, try block throws that exception.</li>
        <li>catch - The catch statement represents a block of code that is executed when a particular exception is thrown from the try block. The code to handle the exception is written inside the catch block.</li>
        <li>throw - An exception in C++ can be thrown using the throw keyword. When a program encounters a throw statement, then it immediately terminates the current function and starts finding a matching catch block to handle the thrown exception.</li></ol></li>
</ul>

}
## Code: 16A
(A) <br> 
```cpp
// NAME - AKALP SARKAR
//PRN - 23070123116
// EXPERIMENT - 16(A) 

// EXCEPTION HANDLING 

#include<iostream>
using namespace std;

int main()
{
    float n1, n2, n3, n4, ans;
    cout<<"Enter values of numbers 1 and 2: ";
    cin>>n1>>n2;
    try{
        if(n2==0) {
            throw n2;
        }
        else {
            ans=n1/n2;
            cout<<"Answer = "<<ans<<endl;
        }
    }
    catch(float num) {
        cout<<"\n ERROR: Division by "<<num<<endl;
    }
}
```

## Output:
![Output16A](https://github.com/user-attachments/assets/8ac88685-e852-46aa-b778-be55f154f3f4)

## Code: 16B
```cpp
// NAME - AKALP SARKAR
// PRN - 23070123116
// EXPERIMENT - 16(B) 

// EXCEPTION HANDLING 

#include<iostream>
using namespace std;

int main()
{
    int age;
    cout<<"Enter age: ";
    cin>>age;
    try{
        if(age<18) {
            throw age;
        }
        else {
            cout<<"Age: "<<age<<"\n APPROVED"<<endl;
        }
    }
    catch(int a) {
        cout<<"\n ERROR: Underage! ("<<age<<")"<<endl;
    }
}

```
## Output:
![Output16B](https://github.com/user-attachments/assets/c6c5f664-f409-4e7f-ae3e-a693278183d7)

### Conclusion:
I learnt about Exception Handling in C++ and about its three keywords: try, catch and throw.
