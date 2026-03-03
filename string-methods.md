# String Methods  
---
###  1 . `string.length()`

```c++
#include <iostream>
using namespace std;
int main() {
    string name;
    cout <<"Enter your name : ";
    getline(cin, name);
    if(name.length() > 12) {
        cout <<"Your name is too long.";
    } else {
        cout <<"Hello, " << name << "!";
    }
    return 0;
}

```
---

### 2. `string.empty()`

```c++
#include <iostream>
using namespace std;
int main() {
    string name;
    cout <<"Enter your name : ";
    getline(cin, name);
   if(name.empty()){
       cout<<"You did not enter your name."<<endl;}
    else{
        cout <<"Hello, " << name << "!" << endl;
    }
    return 0;
}
```
---
### 3.  `String.clear()`
---
### 4. `string.append()`
---
```c++
#include <iostream>
using namespace std;
int main() {
    string name;
    cout <<"Enter your name : ";
    getline(cin, name);
   name.append("@gmail.com");
    cout <<"Your email is : "<<name;
    return 0;
}
```
---

### 5. `string.at(index)`

```c++
#include <iostream>
using namespace std;
int main() {
    string name;
    cout <<"Enter your name : ";
    getline(cin, name);
   cout << name.at(0) << endl;
    return 0;
}
```
---
6. `string.insert()`

```c++
#include <iostream>
using namespace std;
int main() {
    string name;
    cout <<"Enter your name : ";
    getline(cin, name);
   cout << name.insert(0,"@") << endl;
    return 0;
}
```
---
### 7. `string.find(" ")`
---
### 8. `string.erase(beginng_index,ending_index`)
---

#### strig methods in c++

```cpp
#include <iostream>
#include <string>
#include <algorithm>   // Required for reverse()

using namespace std;

int main()
{
    string str = " Ambesh";
    cout << str << endl;

    str.push_back('a');
    cout << str << endl;

    str.pop_back();
    cout << str << endl;

    str.append(" Yadav");
    cout << str << endl;

    str.clear();
    cout << str << endl;

    str = str + "Ambesh Yadav";
    cout << str << endl;

    reverse(str.begin(), str.end());
    cout << str << endl;

    cout<<to_string(12345)<<endl;

    cout<<stoi("12345")<<endl;
    return 0;
}
```

```Output
Ambesh
 Ambesha
 Ambesh
 Ambesh Yadav

Ambesh Yadav
vadaY hsebmA
12345
12345
```
