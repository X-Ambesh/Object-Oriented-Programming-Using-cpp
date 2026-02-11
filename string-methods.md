# String Methods  

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
### 3.  `String.clear()`

### 4. `string.append()`

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

### 7. `string.find(" ")`

### 8. `string.erase(beginng_index,ending_index`)
