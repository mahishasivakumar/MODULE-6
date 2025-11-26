# Ex.No:2
# Ex.Name :Write a CPP program to SORT the Doubly Linked List with 5 elements Using STL and Display the same.
## Date:
## Aim:
To write a C++ program to sort a doubly linked list containing 5 elements using STL list and display the sorted elements.

## Algorithm:
STEP 1: Start the program.

STEP 2: Include the <iostream> and <list> headers.

STEP 3: Declare a list<int> to represent the doubly linked list.

STEP 4: Read 5 integer values from the user.

STEP 5: Use the push_back() function to insert elements at the end of the list.

STEP 6: Call the sort() member function to sort the list in ascending order.

STEP 7: Display a message indicating that the list has been sorted.

STEP 8: Traverse the list using a range-based for loop or iterator.

STEP 9: Print each element during traversal.

STEP 10: End the program.




## Program:
```
#include <iostream>
#include <list>

using namespace std;

int main()
{
    list<int> gqlist1;
    int input;

    for (int i = 0; i < 5; ++i) 
    {
        cin >> input;
        gqlist1.push_back(input);
    }

    gqlist1.sort();

    for (int value : gqlist1)
    {
        cout << value << " ";
    }
    cout << endl;

    return 0;
}

```


## Output:
<img width="606" height="247" alt="{958E8BBF-2F83-41A5-BE67-84CCBC8169B1}" src="https://github.com/user-attachments/assets/9ae2f6ac-bb9a-4e95-b4a7-caf134d70bc1" />



## Result:
The program successfully sorts the doubly linked list using STL and displays the elements in ascending order.

