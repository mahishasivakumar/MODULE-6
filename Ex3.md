# Ex.No:3
# Ex.Name :Write a CPP Program to REMOVE a Node from the Doubly Linked List Using STL and Display the same.
## Date:
## Aim:
To write a C++ program to remove a node from a doubly linked list using STL list and display the updated list.

## Algorithm:
STEP 1: Start the program.

STEP 2: Include the <iostream> and <list> headers.

STEP 3: Declare a list<int> to represent the doubly linked list.

STEP 4: Read 5 integer values from the user and insert them into the list using push_back().

STEP 5: Display the original list.

STEP 6: Ask the user to input the value of the node to remove.

STEP 7: Use the remove() function to delete the node containing the specified value.

STEP 8: Display a message indicating that the node has been removed.

STEP 9: Traverse the updated list using a range-based for loop or iterator.

STEP 10: Print each element and end the program.




## Program:
```
#include <iostream>
#include <list>

using namespace std;

int main() 
{
    list<int> gqlist1;
    int input, elementToRemove;

    for (int i = 0; i < 5; ++i) 
    {
        cin >> input;
        gqlist1.push_back(input);
    }

    cout << "List before removing elements: ";
    
    for (int value : gqlist1)
    {
        cout << value << " ";
    }
    cout << endl;

    cin >> elementToRemove;

    gqlist1.remove(elementToRemove);

    cout << "List after removing elements: ";
    
    for (int value : gqlist1) 
    {
        cout << value << " ";
    }
    cout << endl;

    return 0;
}

```


## Output:
<img width="1171" height="380" alt="{613AFC46-9D35-4CD0-8639-E64C17B11114}" src="https://github.com/user-attachments/assets/186cef6f-ea6a-4a3f-8fbf-c526a73ba6a2" />



## Result:
The program successfully removes the specified node from the doubly linked list using STL and displays the updated list.
