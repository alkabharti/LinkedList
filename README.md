# LinkedList

### Basic Structure of a Linked List :

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


### Initializing a List in Java

List is an interface, and the instances of List can be created in the following ways:

- List a = new ArrayList();
- List b = new LinkedList();
- List c = new Vector(); 
- List d = new Stack(); 



