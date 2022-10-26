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

### Below are the following ways to initialize a list:

### 1. Using List.add() method


```java
public static void main(String[] args){
    // For ArrayList
    List<Integer> list = new ArrayList<Integer>();
    list.add(1);
    list.add(3);
    System.out.println("ArrayList : " + list.toString());

    // For LinkedList
    List<Integer> llist = new LinkedList<Integer>();
    llist.add(2);
    llist.add(4);
    System.out.println("LinkedList : " + llist.toString());

    // For Stack
    List<Integer> stack = new Stack<Integer>();
    stack.add(3);
    stack.add(1);
    System.out.println("Stack : " + stack.toString());

    }

    /*
    Output :
    ArrayList : [1, 3]
    LinkedList : [2, 4]
    Stack : [3, 1]

    */

```

- **Double Brace Initialization** can also be used to do the above work.


```java
public static void main(String args[])
{

    // For ArrayList
    List<Integer> list = new ArrayList<Integer>() {{
        add(1);
        add(3);
        } };
    System.out.println("ArrayList : " + list.toString());

    // For LinkedList
    List<Integer> llist = new LinkedList<Integer>() {{
        add(2);
        add(4);
        } };
    System.out.println("LinkedList : " + llist.toString());

    // For Stack
    List<Integer> stack = new Stack<Integer>() {{
        add(3);
        add(1);
        } };
    System.out.println("Stack : " + stack.toString());
}

/*

Output:
ArrayList : [1, 3]
LinkedList : [2, 4]
Stack : [3, 1]

*/

```






