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

#### To find the sum of elements in an array

```cpp
#include <iostream>
using namespace std;
int main() {
    int arr[] = {1, 2, 3, 4, 5};
    int n = sizeof(arr) / sizeof(arr[0]);
    int sum = 0;
    for (int i = 0; i < n; i++) {
        sum += arr[i];
    }
    cout << "Sum of array elements: " << sum << endl;
}
```

---

#### To find the max number in an array

```cpp
#include <iostream>
using namespace std;
int main() {
    int arr[] = {67, 27, 12, 97, 66};
    int n = sizeof(arr) / sizeof(arr[0]);
    int mx = arr[0];
    for (int i = 1; i < n; i++) {
        mx = max(mx,arr[i]);
    }
    cout << "Max Number in this array is " << mx;
}
```

---

#### To print a 2d 

```cpp
#include <iostream>
using namespace std;
int main(){
    int arr[4][4]={{1,2,3,4},
                 {5,6,7,8},
                 {9,10,11,12},
                 {13,14,15,16}};
}
```

---

#### To find transpose of a matrix

```cpp
#include <iostream>
using namespace std;
int main()
{
    int arry[4][3] = {
        {1, 2, 3},
        {4, 5, 6},
        {7, 8, 9},
        {10, 11, 12}};
    for (int j = 0; j < 3; j++)
    {
        for (int i = 0; i < 4; i++)
        {
            cout << arry[i][j] << " ";
        }
        cout << endl;
    }
}
```

>Output:

```Output:
1 4 7 10 
2 5 8 11 
3 6 9 12 
```

---

#### Make a 2d matrix of 5X4 and store 10 as every element

```cpp
#include <iostream>
using namespace std;
int main() {
    int arr[5][4];
    for(int i=0;i<5;i++){
        for(int j=0; j<4;j++){
            arr[i][j]=10;
            cout <<arr[i][j]<< " ";}
        cout << endl;
    
    }
}
```

>Output

```Output:
10 10 10 10 
10 10 10 10 
10 10 10 10 
10 10 10 10 
10 10 10 10 
```

---
