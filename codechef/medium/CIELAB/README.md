# CIELAB

![Difficulty](https://img.shields.io/badge/Difficulty-Medium-yellow)

## Problem

### Ciel and A-B Problem

In Ciel's restaurant, a waiter is training. Since the waiter isn't good at arithmetic, sometimes he gives guests wrong change. Ciel gives him a simple problem. What is  **A** - **B**  (**A**  minus  **B**) ?

Surprisingly, his answer is wrong. To be more precise, his answer has exactly one wrong digit. Can you imagine this? Can you make the same mistake in this problem?

### Input

An input contains 2 integers  **A**  and  **B**.

### Output

Print a wrong answer of  **A** - **B**. Your answer must be a  *positive*  integer containing the same number of digits as the correct answer, and exactly one digit must differ from the correct answer. Leading zeros are not allowed. If there are multiple answers satisfying the above conditions, anyone will do.

### Constraints

1 ≤  **B**  <  **A**  ≤ 10000

### Sample 1:
Input
Output

```
5858 1234
```

```
1624
```

### Explanation:

The correct answer of 5858-1234 is 4624. So, for instance, 2624, 4324, 4623, 4604 and 4629 will be accepted, but 0624, 624, 5858, 4624 and 04624 will be rejected.

### Notes

The problem setter is also not good at arithmetic.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-10-30T06:32:31.971Z  

```c_cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
	// your code goes here
long long a, b;
cin>>a>>b;
long long c = a-b;
int d = c%10;
if(d<9){
    cout<<c+1;
}
else{
    cout<<c-1<<endl;
}
}
```

---

[View on CodeChef](https://www.codechef.com/problems/CIELAB)