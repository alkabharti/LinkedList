<h2> Reverse a linked list :</h2>

Given a linked list of N nodes. The task is to reverse this list.

**Example 1:**

Input: <br/>
LinkedList: 1->2->3->4->5->6 <br/>
Output: 6 5 4 3 2 1 <br/>
Explanation: After reversing the list, elements are 6->5->4->3->2->1.

**Example 2:**

Input: <br/>
LinkedList: 2->7->8->9->10 <br/>
Output: 10 9 8 7 2 <br/>
Explanation: After reversing the list, elements are 10->9->8->7->2.

**Link :** https://practice.geeksforgeeks.org/problems/reverse-a-linked-list/1

-------------------------------------------------------------------------------------------------------------------------------------------


<h3> Solution : </h3>

Time Complexity :

```java
Node reverseList(Node head)
{
    Node current=head;
    Node prev=null;
    Node next=null;
    while(current!=null)
    {
        next=current.next;
        current.next=prev;
        prev=current;
        current=next;
    }
    return prev;
}
```


