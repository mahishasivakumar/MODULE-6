# Ex.No:1
# Ex.Name Write a CPP program to INSERT 5 elements into the Singly Linked List Using STL and Display the same.
# Date:
## Aim:
To write a C++ program to insert 5 elements into a singly linked list using STL forward_list and display the elements.

## Algorithm:
STEP 1: Start the program.

STEP 2: Include the <iostream> and <forward_list> headers.

STEP 3: Declare a forward_list<int> to represent the singly linked list.

STEP 4: Read 5 integer values from the user.

STEP 5: Use the push_front() function to insert elements at the beginning of the list.

STEP 6: Alternatively, use insert_after() for inserting at the end if order matters.

STEP 7: Display a message indicating that elements are inserted.

STEP 8: Traverse the singly linked list using a range-based for loop.

STEP 9: Print each element during traversal.

STEP 10: End the program.




## Program:
```
#include <iostream>
#include <forward_list>

using namespace std;

int main()
{
    forward_list<int> sll;

    sll.push_front(50);
    sll.push_front(40);
    sll.push_front(30);
    sll.push_front(20);
    sll.push_front(10);

    cout << "The forward list operation: ";
    
    for (const int& elem : sll) 
    {
        cout << elem << " ";
    }
}

```


## Output:
<img width="922" height="151" alt="{665BBBAE-BCE4-4B73-9CFA-53DC4CD2DCFF}" src="https://github.com/user-attachments/assets/75097492-79da-4777-b1db-b4abf9903273" />



## Result:
The program successfully inserts 5 elements into the singly linked list using STL and displays them in the list order.
