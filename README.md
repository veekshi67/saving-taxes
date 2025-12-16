# Saving Taxes

This repository contains a C++ solution for the **Saving Taxes** problem.

---

## 🧩 Problem Statement

In Chefland, anyone earning **strictly more than Y rupees** must pay tax.  
Chef allows an exemption scheme where you can invest any amount to reduce your taxable income.

Given:
- `X` = total income
- `Y` = tax threshold (`X > Y`)

Find the **minimum amount** that must be invested so that no tax is paid.

---

## 💡 Logic

To avoid tax:
Effective income ≤ Y


So the minimum investment required is:


Investment = X - Y


---

## ✅ Example

**Input**


4
4 2
8 7
5 1
2 1


**Output**


2
1
4
1


---

## ⏱ Complexity

- **Time Complexity:** `O(T)`
- **Space Complexity:** `O(1)`

---

## 💻 C++ Implementation

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int t;
    cin >> t;
    while (t--) {
        int x, y;
        cin >> x >> y;
        cout << x - y << endl;
    }
    return 0;
}

⭐ Conclusion

A simple arithmetic-based solution that efficiently determines the minimum investment required to avoid tax.
