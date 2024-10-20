# exception-handling
# Experiment- 16
## Aim- To study and implement exception handling
## Theory-
In C++, exception handling is an essential mechanism that helps manage unexpected runtime errors by controlling the program flow in response to these errors. It is built around three main keywords:
Keywords of Exception Handling:
throw: This keyword is used to signal that an error has occurred during program execution. When an exception is thrown, the current function exits, and the control is transferred to a catch block that can handle the exception. Various types of values, such as integers, strings, or even objects, can be thrown as exceptions.
catch: This keyword defines the block of code that will handle the thrown exception. Each catch block specifies a particular type of exception it can handle, and it only catches exceptions of that type. If no matching catch block is found, the program terminates.
try: The try block contains code that might throw an exception. It acts as a guard, and when an exception is thrown inside the try block, control is transferred to the appropriate catch block.
Flow of Exception Handling:
When an exception occurs within a try block, the program flow is interrupted, and the exception is thrown.
Control is passed to the catch block that matches the type of the thrown exception.
If the exception is successfully caught, the catch block handles the error, and the program can either continue or terminate based on the handling logic.
If no matching catch block is found, the program will terminate unexpectedly.

##Code
~~~
#include <iostream>
using namespace std;

int main() 
{
    int den,num;
    float ans;

    cout << "Enter the numerator: ";
    cin >> num;
    cout << "Enter the denominator: ";
    cin >> den;

    try 
    {
        if (den == 0) 
        {
            throw 0;  
        }

        cout << "Answer: "<< num/den << endl;
    }

    catch (int x) 
    {
        cout << "ERROR: DIVISION BY ZERO" << endl;
    }

}
~~~
## Output-
![](https://github.com/SunidhiChoubey/exception-handling/blob/main/Screenshot%202024-10-21%20020234.png)
## Conclusion-
We learnt about exception handling in C++ and We learnt the flow of exception handling in C++.

