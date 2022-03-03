# LinkedList

Basic Structure of a Linked List :

Like arrays, Linked List is a linear data structure. Unlike arrays, linked list elements are not stored at the contiguous location, the elements are linked using pointers.

```java
class LinkedList
{
    Node head;  //Head of list
    class Node   //Node class
    {
        int data;
        Node next;
        Node(int d)
        {
            data=d;
            next=null;
        }
    }
}
```

