# Ex.No:4
# Ex.Name :Write a CPP program to INSERT 5 elements into the Circularly Linked List and Display the same.
## Date:
## Aim:
To write a C++ program to insert 5 elements into a circular linked list and display the list.

## Algorithm:
STEP 1: Start the program.

STEP 2: Create a Node structure with data and a next pointer.

STEP 3: Declare a pointer head to keep track of the start of the circular linked list.

STEP 4: Initialize head as nullptr.

STEP 5: Read 5 integer values from the user.

STEP 6: For each value, create a new node and insert it into the circular linked list.

STEP 7: If the list is empty, set head to the new node and point next to itself.

STEP 8: Otherwise, traverse to the last node and insert the new node after it, maintaining circularity.

STEP 9: Display the elements by traversing the circular list starting from head until we reach head again.

STEP 10: End the program.




## Program:
```
#include<iostream>
using namespace std;

class Node
{
    public:
    int data;
    Node *nextptr;
}*head,*tail,*newn,*temp;

void display()
{
    temp = head;
    do
    {
        cout<<"Data = "<<temp->data<<" ";
        temp = temp->nextptr;
    }
    while(temp->nextptr!=head);
    cout<<"Data = "<<temp->data<<" ";
    cout<<endl;
}

void createNode(int n)
{
    newn = new Node();
    newn->data = n;
    newn->nextptr = 0;
    
    if(head==0)
    {
        head = newn;
        tail = newn;
    }
    
    else
    {
        tail->nextptr = newn;
        tail = newn;
        tail->nextptr = head;
    }
}

int main()
{
    int n;
    for(int i=0;i<5;i++)
    {
        cin>>n;
        createNode(n);
    }
    
    display();
}
```


## Output:
<img width="1184" height="337" alt="{9D3328DC-BE14-40F0-B0F1-BCC099678C32}" src="https://github.com/user-attachments/assets/7086d5b7-35e0-4fbe-ab87-a313aba405f3" />



## Result:
The program successfully inserts 5 elements into a circular linked list and displays the list in the correct order.
