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


#include<iostream>
using namespace std;
 
int main(){
    int arr[]={10,20,30,40,50};
    int n=sizeof (arr)/ sizeof(arr[0]);
    int low=0;
    int high=n-1;
    int val=50;
    int index=-1;
    while(low<= high){
        int mid=(low+high)/2;
        if (arr[mid]==val){
            index=mid;
            break;
        }
        else if (arr[mid]<val){
            low=mid+1;
        }
        else{
            high=mid-1;
        }
    }
    if (index==-1){
        cout<<"not found"<<endl;
    }
    else{ 
        cout<< "found at index "<<index<<endl;
    }
}
