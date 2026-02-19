C++  important questions 

### combinations

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

### To swap two numbers without using third variable

```cpp
#include <iostream>
using namespace std;
int main(){
    int x,y;
    cout<<"Enter two numbers: ";
    cin>>x>>y;
    x=x+y;
    y=x-y;
    x=x-y;
    cout<<"After swapping: "<<x<<" "<<y;
}
```

---

### Write a code to print sum of even digits and product of odd digits of a number.

```c++
#include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    int even =0;
    int odd =1;
    while (num > 0) {
        int digit = num % 10;
        if (digit % 2 == 0) {
            even += digit;
        }
        else {
            odd *= digit;
        }
        num /= 10;
    }
    cout << "Sum of even digits:  " << even << endl; ;
    cout << "Product of odd digits:  " << odd << endl;
    return  0;
}
```

###  To print factorial of a number.
   
```c++
  #include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    int fac=1;
    for(int i=1; i<=num; i++)
        fac *= i;
    cout << "Factorial of " << num << " is: " << fac << endl;
    return 0;
} 
```
### To reverse a number 
```c++
#include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    int rev=0;
    while (num > 0) {
        rev = rev * 10 + num % 10;
        num /= 10;
    }
    cout << "Reversed number: " << rev << endl;
    return 0;
}
```

### To check weather a number is palidrome or not 

```c++
#include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    int rev = 0;
    while (num > 0) {
        rev = rev * 10 + num % 10;
        num /= 10;
    }
    if (rev == num) {
        cout << "The number is a palindrome." << endl;
    } else {
        cout << "The number is not a palindrome." << endl;
    }
    return 0;
}
```
### To check weather a number is prime or not 

```c++
#include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    int p = 0;
    for (int i = 1; i <= num; i++) {
        if (num % i == 0) {
        p += 1;}
    }
    if (p > 2) {
        cout << "The number is not prime." << endl;
    } else {
        cout << "The number is prime." << endl;
    }
    return 0;
}
```

### To print table of a number

```c++
#include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    for(int i = 1; i <=10; i++){
        cout << num << " x " << i << " = " << num * i << endl;
    }
    return 0;
}
```

### To generate a fibonacci series upto a given number 

```c++
#include <iostream>
using namespace std;
int main() {
    int a = 0;
    int b = 1;
    int num;
    cout << "Enter the number of Fibonacci numbers to generate: ";
    cin >> num;
    cout << "Fibonacci sequence: ";
    for (int i = 0; i < num; i++) {
        cout << a << " ";
        int next = a + b;
        a = b;
        b = next;}
    return 0;
          
}
```

### Write a program to find $x^y$

```c++
#include <iostream>
using namespace std;
int main() {
    int x , y ;
    cout << "Enter two numbers: ";
    cin >> x >> y ;
    int ans = 1;
    for (int i=1; i<=y; i++){
        ans*=x;}
    cout << x << "^" << y << " = " << ans;
    return 0;  
}
```

###  
