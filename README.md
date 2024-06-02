# C and Python and C++ speed comparation

c is faster than python.
python is faster than c++.

```
c++
Total runtime: 0:00:00:0.2278

c
Total runtime: 0:00:00:0.0433

python
Total runtime: 0:00:00:0.1107
```

> If c++ is slower than c, then [java, rust, javascript/typescript, c#, dart, kotlin] would all be slower than c.

> In other words, for c, if a task will take 1 day to finish, then, for all other programming language, it would take 2 to 10 days.

## How to test?
```
./test.sh
```

## Code
```
//c
//gcc c_main.c -o c_main.run

int main() 
{ 
    int n = 777600; 
  
    int vect[n];
  
    int i = 0;
    for (i; i<n; i++) {
        vect[i] = 1;
    }
  
    return 0; 
}
```

```
//c++
//g++ cpp_main.c -o cpp_main.run

#include <vector> 
using namespace std; 
  
int main() 
{ 
    int n = 777600; 
  
    vector<int> vect(n);
  
    int i = 0;
    for (i; i<n; i++) {
        vect[i] = 1;
    }
  
    return 0; 
}
```

```
#python
#python3 python_main.py

n = 777600;
a_list = [None] * n
for i in range(n):
    a_list[i] = 1
```

## Author
yingshaoxo
