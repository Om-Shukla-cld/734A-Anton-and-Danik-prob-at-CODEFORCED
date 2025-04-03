# 734A-Anton-and-Danik-prob-at-CODEFORCES
#include <bits/stdc++.h>
using namespace std;

int main() {
    int n;
    string m;
    cin >> n;  // Read the number of games
    cin >> m;  // Read the game result string

    int c = 0, d = 0;

    for (int i = 0; i < n; i++) {  // Start loop from i = 0 (zero-based indexing)
        if (m[i] == 'D')  // Use single quotes for character comparison
            c++;
        else if (m[i] == 'A')  // Correctly handle the "Anton" case
            d++;
    }

    if (c > d) 
        cout << "Danik" << endl;
    else if (d > c)
        cout << "Anton" << endl;
    else 
        cout << "Friendship" << endl;  // If they are equal

    return 0;
}
