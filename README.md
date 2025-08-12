#include<iostream>
using namespace std;

int main() {
    int arr[] = {2, 5, 6, 10, 20};
    int val = 2;
    int index = -1;
    int n = sizeof(arr) / sizeof(arr[0]);  // Correct way to find array size

    for (int i = 0; i < n; i++) {
        if (arr[i] == val) {
            index = i;
            break;  // Exit loop once value is found
        }
    }

    if (index == -1) {
        cout << "Not found" << endl;
    } else {
        cout << "Found at index " << index << endl;
    }

    return 0;
}

