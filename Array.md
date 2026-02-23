### Arrays

---

#### To input elements of array

```cpp
#include <iostream>
using namespace std;
int main() {
    int x[5];
    for(int i = 0; i < 5; i++) {
        cout << "Enter array element " << i+1 << ": ";
        cin >> x[i];
    }
    for(int i = 0; i < 5; i++) {
        cout << x[i] << " ";
    }
    cout << endl;
}
```

---

#### Arrays are by default pass by reference

```cpp
#include <iostream>
using namespace std;
void change(int x[]){
    x[0] = 100;
}
int main(){
    int x[5] = {1, 2, 3, 4, 5};
    change(x);
    for(int i = 0; i < 5; i++){
        cout << x[i] << " ";// Output: 100 2 3 4 5
    }
    cout << endl;
    return 0;
}
```

---
