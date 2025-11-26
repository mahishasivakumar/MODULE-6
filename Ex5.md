# Ex.No:5
# Ex.Name :Write a C++ function int printList(Node *head) to print the polynomial expression in polynomial addition program using Linked list concept.
## Date:
## Aim:
To write a C++ function int printList(Node *head) to display a polynomial expression stored in a linked list, where each node contains a coefficient and exponent (power).

## Algorithm:
STEP 1: Start the program.

STEP 2: Define a Node structure with members:

coeff → coefficient of the term

power → exponent of the term

next → pointer to the next node

STEP 3: Initialize the head pointer of the linked list.

STEP 4: Display a heading like "Linked List".

STEP 5: Traverse the linked list starting from head.

STEP 6: For each node, print the coefficient followed by "x^" and the exponent (power).

STEP 7: Move to the next node using head = head->next.

STEP 8: Repeat steps 6-7 until the end of the list (head == NULL).

STEP 9: Return 1 to indicate the function executed successfully.

STEP 10: End the program.




## Program:
```
int printList(Node *head)
{
    
    cout << "Linked List" << endl;
  
    while(head != NULL)
    {
        cout << " " << head->coeff <<"x" << "^" << head->power;
        head = head->next;
    }
    
    return 1;
}

```


## Output:
<img width="503" height="252" alt="{E891058C-7EA2-4AE5-97DB-862243343EC2}" src="https://github.com/user-attachments/assets/f3367f17-8b21-4634-8b92-7f0c9b95cd87" />



## Result:
The function successfully prints the polynomial expression in the form:

Linked List
 5x^3 4x^2 2x^0

for any linked list representing polynomial terms.
