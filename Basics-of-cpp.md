### Tokens in cpp

> Tokens are smallest individual enlement of a   programing languge.
>
>Tokens are caterised into :
>
> K >>>  Keyword  
> I >>> identifer   
> L >>> Lierals/constants   
>  P/S >>>Punctuators/Seperators  
> O >>> Operators  

Tokens

- Keywords : Reserved words by a programing language   
    - Example : if, while, for, float, char, double 
- Identifier : Are the names given to variables / class / function 

    - Example ` int a = 5;`

        - int = Keyword
        - a = identifier > Variable
    - Rules for identifiers
     
        - Keywords can't be used as identifiers.
        - First character must be alphabet or underscore ( _ ).
        - No symboles except underscore ( _ )is allowed. 
        - NO space is allowed between names.
        - Identifiers are case sensetive.
- Literals/constants
    
    Literals/Constants are fixed values whose value cannot be changed during the execuation of the program.

    - Const : create a constant variable
        - Exmple : 

        ```c++ 
        const int a = 10 ;   
        a = 20 // Error ;
        ```
 

- Punctuators/seperators 

  It seperates one elements from other.
    - Eample 

            int a,b;
            float x,y;
            \\; , (,) ,"",[],(),'',{} etc are punctuators.

- Operators 
    - To perform specific operations 
    - Arthemetic operators
        - (+),(-),(*),(/),(%)
    - Relatioal Operators 
         - (>,<,>=,<=,==,!=)
    - Assignment operators
        - =
        - Short hand assignment operators
            - +=, -= ,*= ,/= , %=
    - Increment / Decrement operator
        - a++ postfix
        - a-- postfix
        - --a prefix
        - ++a prefix
    - Logical Operator
        - and (&&) ex (a>b) && (a>c)
        - or (||)  ex (a>b) || (a>c)
        - not (!)  ex !(a>c)
    - Conditional  operators  
        - ?
        - : 
            - example
            
                     c=a>b?a:b;
### Datatypes

- User-defined data types
    - Structure
    - Union 
    - Class

- built-in data types
    - Integral
        - int 
        - long

    - void 
    - floting 
        - float
        - dubble

- derived data types
    - String 
    - Array

### Basic Structure of cpp  

- preprocessor directive 

         #include<iostream.h>
- class 

        class class_name(){}
- Function

             int main(){
                //statements
                ____________;
                ____________;
                return 0;
             }


### Cin and Cout in cpp
- cin it is used to take input

        int a;
        cout << " Enter a value;
        cin >> a;
        int x,y;
        cin >> a>> b;
- cout it is used to display output

            cout << "welcome to cpp";

### Programs

#### WAP to add two numbers

    #include<iostream.h>
    int main(){
        int a, b ,c ; 
        cout << "Enter two numbers ";
        cin >> a >> b;
        cout << "addition = ">> a+b;
        return 0;
    }

#### To calculate percentage

    #include <iostream>
    using namespace std;

    int main()
    {
        int phy, maths, chem, cs, eng;
        cout << "Enter marks of physics : ";
        cin >> phy;
        cout << " Enter the marks of maths : ";
        cin >> maths;
        cout << "Enter the marks of chem : ";
        cin >> chem;
        cout << "Enter the marks of CS : ";
        cin >> cs;
        cout << "Enter the marks of english : ";
        cin >> eng;
        int total_marks = phy + maths + chem + cs + eng;
        cout << "The Total marks are: " << total_marks;
        cout << "Total percentage is " << (total_marks / 500.0) * 100;
        return 0;
        }

### Control statements 

Control statements are used to control the flow of </br>
 execution of a program

- Selection Control statements
    - if else

            if (codition)
            ___________;
            if (condition){
            _____________;
            _____________;
            _____________;}
            else if (condition)
            _________________;
            else
            ____________;
    - switch

- Iterative/loping control 
    - while
    - do while
    - for 
- jump statements
    - break
    - contiue
    - goto
#### To check weather the number is odd or even
```c++
#include<iostream>
using namespace std;
int main(){
    int a;
    cout<<"Enter a number : ";
    cin >> a ;
    if ( a % 2 == 0)
        cout<< "The number is even ";
    else
        cout<<"The number is odd ";
    return 0;

}
```

#### To find the gratest number among three

```c++
#include <iostream>
using namespace std;
int main()
{
int a,b,c;
cout << "Enter number a,b,c : ";
cin >> a >> b >> c;
if ((a>b)&&(a>c))
cout << "Max number is a ";
else if ((b>a)&&(b>c))
    cout << "Max nummber is b ";
else 
    cout << "Max number is c ";
return 0;
}
```

### To find sum of digits of a number 

```c++
#include <iostream>
using namespace std;
int main() {
    int a;
int sum = 0;
cout << "Enter a number: ";
cin >> a;
while (a>0) {
    sum+=a%10;
        a/=10;
}
return 0;
}
```




        
# Object-oriented-programing-with-c++

# Q1. Write a C++ program that takes two integers as input from the user and displays their sum.

```c++
#include <iostream>
int main(){
int a,b,c;
std::cout<<"\nEnter a  and b";
std::cin>>a>>b;
c=a+b;
std::cout<<c;
return 0;
}```
# Q2. Write a C++ program to check whether a given number is even or odd.
    #include <iostream>
    int main()
    {
    int a;
    std::cout << "Enter a number: ";
    std::cin >> a;

    if (a % 2 == 0) {
        std::cout << "Even number\n";
    } else {
        std::cout << "Odd number\n";
    }
    return 0;
    }
```

# Q3. Write a C++ program to print all numbers from 1 to n, where n is a number entered by the user.

```c++
#include <iostream>
using namespace std;

int main() {
int n;
cin >> n;
for (int i = 1; i <= n; i++)
{
cout << i << " ";
}
return 0;
}
```
# Q4. To print sum of n natural numbers

```c++
#include <iostream>
using namespace std;

int main(int argc, char *argv[])
{
    int n, sum = 0;

    if (argc > 1)
        n = atoi(argv[1]);
    else {
        cout << "Enter n: ";
        cin >> n;
    }

    for (int i = 1; i <= n; i++)
        sum += i;

    cout << "Sum = " << sum;
    return 0;
}
```

# WAP to swap two values 

```c++
#include <iostream>
void swap(std::string &a, std::string &b){
    std::string temp;
    temp=a;
    a=b;
    b=temp;
}
int main(){
std::string x = "Kool aid";
std::string y = "Water";
std::string temp;
swap(x,y);
std::cout<<x <<"\n";
std::cout<<y <<"\n";
}
```
## Outuput
    Water
    Kool aid


#### This is the end of file

### Break and continue in cpp

  > Break in c++

```c++
#include <iostream>
using namespace std;
int main() { 
    int i = 0;
    while (i <= 10) {
        if (i == 5) {           
            break;
        }
        cout << i << " ";
    }
    return 0;
}
```

> continue in c++

```c++
#include <iostream>
using namespace std;
int main() { 
    int i = 0;
    while (i <= 10) {
        
        if (i == 5) { 
            i++;          
            continue;
        }
        cout << i << " ";
        i++;
    }
    return 0;
}
```

### Go to statement in c++

>  goto statement is a type of jump contorol statement 
> used to transfer the flow of execution of the program

```C++
#include <iostream>
using namespace std;
int main() { 
    int i;
    cout << "Enter an number : ";
    cin >> i;
    if (i % 2 == 0) {
        goto even;
    } else {
        goto odd;
    }
even:
    cout << "The number is even." << endl;
    return 0;
odd:
    cout << "The number is odd." << endl;
    return 0;
}
```

---

### Pre increment and post increment 

> Pre increment
```c++
int x = 4;
cout << x;// 4
cout << ++x<< endl; // 5
cout << x << endl; // 5
```

> Post increment 
```c++
int x = 4;
cout << x;// 4
cout << x++ << endl; // 4
cout << x << endl; // 5
```
---
### Use of modulus Operator. 
```c++
a % b = a  // [if a < b ]
a % a = 0 
a % (-b) = a % b 
(-a) % b = -(a % b) 
```
---

### Type-casting
```c++
#include <iostream>
using namespace std;
int main() {
    int x;
    cout << "Enter an integer: ";
    cin >> x;
    float y = (float)x;
    cout << "Half of " << x << " is " << y/2 << endl;
}
```
---
### Hierarchy of operations 
> `B | O | DM | A | S` # Left to right

```c++
#include <iostream>
using namespace std;
int main() {
    int i = 2*3/4;
    cout << i << endl;
    return 0;
}
// Output : 1 
```
---

### ASCII Values


ASCII Values |
---------|
 a --> 97 |
 A --> 65 |
 0--> 48 |

> To print ASCII Values

```c++
#include <iostream>
using namespace std;
int main() {
    char ch;
    cout << "Enter a character: ";
    cin >> ch;
    cout<<(int)ch;
    return 0;
}
```

> Integer to ASCII 
```c++
#include <iostream>
using namespace std;
int main() {
    int x;
    cout << "Enter a character: ";
    cin >> x;
    cout<<(char)x;
    return 0;
}
```

---

### Important things to remember

```c++

#include <iostream>
using namespace std;
int main() {
    cout << 5/2 << endl; // Outputs 2, because both 5 and 2 are integers
    cout << 5.0/2 << endl; // Outputs 2.5, because 5.0 is a double
    cout << 5/2.0 << endl; // Outputs 2.5, because 2.0 is a double
    cout << 5.0/2.0 << endl; // Outputs 2.5, because both 5.0 and 2.0 are doubles
    return 0;
}
```

---

```c++
#include <iostream>
using namespace std;
int main() {
   cout << (float)(7/22*(3.14+2)*3/5) << endl;// Output 0
    return 0;
}
```

---

### find the greatest number among three by using nested if else

```c++
#include <iostream>
using namespace std;
int main() {
   int a,b,c;
   cout << "Enter a number a : ";
   cin >> a;
   cout << "Enter a number b : ";
    cin >> b;
    cout << "Enter a number c : ";
    cin >> c;
    if(a>b){
        if(a>c)
            cout << a << " is the greatest number.";
        else // c>a ,a>b --> c>a>b
            cout << c << " is the greatest number.";
    }
    else{ // b>a
        if(b>c)
            cout << b << " is the greatest number.";
        else // c>b , b>a --> c>b>a
            cout << c << " is the greatest number.";
    }

    return 0;
}
```

---

### Ternary Operator 

>` //(condition)  ? if true : if false ;`

```c++
#include <iostream>
using namespace std;
int main() {
    int n;
    cout << "Enter n: ";
    cin >> n;
    //(condition)  ? if true : if false ;
    (n%2==0) ? cout << "even " : cout << "odd ";
    return 0;
}
```

---

### Switch Statement

```c++
#include <iostream>
using namespace std;
int main() {
    int x;
    cout << "Enter x ";
    cin >> x;
    char op;
   cout << "Enter operator ";
    cin >> op;
    int y;
    cout << "Enter y ";
    cin >> y;
    switch(op) {
        case '+':
            cout << x+y;
            break;
        case '-':
            cout << x-y;
            break;
        case '*':
            cout << x*y;
            break;
        case '/':
            cout << x/y;
            break;
        default:
            cout << "Invalid operator";
        return 0;
    }
}
```

---

### Predict the output

```c++
#include <iostream>
using namespace std;
int main() {
    int x=3,y,z;
    y=x=10; // Right to left
    z=x<10; // 0 for false and 1 for true
    cout<<x<<"  "<<y<<"  "<<z; 
}
```

> Output `10 10 0`

---

### Continue Statement

```c++
#include <iostream>
using namespace std;
int main() {
    for(int i = 1; i <=20 ; i++){
        if(i==3 || i==8)
            continue;
        else
            cout << i << " "; 
    }
}
```

---

### To find the reverse of a number 

```c++
#include <iostream>
using namespace std;
int main() {
    int x;
    cout << "Enter a number to find the reverse ";
    cin >> x;   
    int rev = 0;
    while (x > 0) {
        rev = rev * 10 + x % 10;
        x = x / 10;
    
    }
    cout << "The reverse of the number is: " << rev << endl;
    return 0;
}
```

---

### To print pattern.

>```
>ABCDE
>ABCDE
>ABCDE
>```

```c++
#include <iostream>
using namespace std;
int main() {
    for(int i = 1; i <=3; i++){
        for(int j = 1; j <=5; j++){
            cout <<(char)(64+j);
        }         
        cout << endl;
    }
    return 0;
}
```

---

### To print upright triangle

```c++
#include <iostream>
using namespace std;
int main() {
    for (int i = 1; i <= 4; i++) {
        for (int j = 1; j <=i; j++) {
            cout<<"*";
        }
        cout<<endl;
    }
}
```
>output 

```
*
**  
*** 
****
```

---

### To print 

```
A
AB
ABC
ABCD
```

```c++
#include <iostream>
using namespace std;
int main() {
    for (int i = 1; i <= 4; i++) {
        for (int j = 1; j <=i; j++) {
           cout<<(char)(64+j);
        }
        cout<<endl;
    }
}
```

---

### Write a code to print

```********    
*******     
******
*****
****
***
**
*
```

```c++
#include <iostream>
using namespace std;
int main() {
    int n;
    cout << "Enter n : ";
    cin >> n;
    for (int i = 1; i <= n; i++) {
        for (int j = 1; j <= n-i+1; j++) {
           cout<<"*";
        }
        cout<<endl;
    }
}
```

---

### Functions

> `main()` It cannot be called more than once
> 
> `return;` Any statement bellow this will not be executed
>
> `int()` We can return value
> 
> `void()` We can store value

```cpp
void sum(int a , int b ){ // (int a , int b) are formal paramters
    cout<<a+b;
}
int main(){
    sum(67,30) // 67,30 are actual parameters and this is pass by value
}
```

---

### Sum of two numbers 
```cpp
#include <iostream>
using namespace std;
int sum(int a, int b){
    return a+b;
}
int main(){
    int a;
    cout<<"Enter Number a : ";
    cin>>a;
    int b;
    cout<<"Enter Number b : ";
    cin>>b;
    cout << sum(a, b);
    return 0;
}
```

---

### Library functions 

Example

>`sqrt()`
>
>`max()`

### To find squareroot, cuberoot,min,max,pow

```cpp
#include <iostream>
#include <cmath>
using namespace std;
int main(){
    cout << sqrt(4);
    cout << cbrt(8);
    cout << min(4,8);
    cout << max(4,8);
    cout << pow(2,10);
}
```

### Permuntation and combinations

${}^nC_r$ = $\frac{n!}{r!(n-r)!}$

```cpp
#include <iostream>
using namespace std;
int fac(int x){
    int a = 1;
    for(int i=1;i<=x;i++){
        a = a*i;
    }
    return a;
}
int main(){
    int n,r;
    cout <<"Enter n & r :  ";
    cin>>n>>r;
    cout << "nCr = " << fac(n)/(fac(r)*fac(n-r)) << endl;
    return 0;
}
```

---

### Pass by value and pass by reference

### Pass by value

```cpp
#include <iostream>
using namespace std;
int swap(int a, int b){
    int temp;
    temp=a;
    a=b;
    b=temp;
    return a,b;
}
int main(){
    int x,y;
    cout<<"Enter two numbers: ";
    cin>>x>>y;
    swap(x,y);
    cout<<"After swapping: "<<x<<" "<<y; //No change x=x & y=y
}
```

---

### Pass by reference

```cpp
#include <iostream>
using namespace std;
int swap(int& a, int& b){
    int temp;
    temp=a;
    a=b;
    b=temp;
    return a,b;
}
int main(){
    int x,y;
    cout<<"Enter two numbers: ";
    cin>>x>>y;
    swap(x,y);
    cout<<"After swapping: "<<x<<" "<<y;//Change x=y & y=x 
}
```

---

### To print address

```cpp
#include <iostream>
using namespace std;
int main(){
    int x = 3;
    int y = 3;
    cout<<&x<<endl;
    cout<<&y<<endl;
```

>`Output`
>
>0xa7ec3ff93c
>
>0xa7ec3ff938

---

### To store address

```cpp
#include <iostream>
using namespace std;
int main(){
    int x = 3;
    int*p = &x;
    cout<<&x<<endl;
    cout<<p<<endl;
    cout<<*p<<endl;

}
```

>`Output`
>
>0x6839bff674
>
>0x6839bff674
>
>

---
