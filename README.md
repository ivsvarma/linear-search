# linear-search
#include <iostream>
using namespace std;

int linearSearch(int arr[], int n, int target) {
    for (int i = 0; i < n; i++) {
        if (arr[i] == target) {
            return i;
        }
    }
    return -1; // target not found
}

int main() {
    int arr[] = {5, 2, 9, 1, 7};
    int n = sizeof(arr) / sizeof(arr[0]);
    int target = 9;
    int result = linearSearch(arr, n, target);
    if (result == -1) {
        cout << "Target not found" << endl;
    } else {
        cout << "Target found at index " << result << endl;
    }
    return 0;
}
