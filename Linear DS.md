# Notes
- https://leetcode.com/problems/remove-nth-node-from-end-of-list
- https://leetcode.com/problems/odd-even-linked-list/
- https://leetcode.com/problems/merge-k-sorted-lists/

# Linked List

## Algorithms
1. Floyd Cycle Detection (FCD)<br>
   1. slow = slow -> next, fast = fast->next->next
   2. if(slow == fast) "cycle" else (fast == null) "no cycle"<br>
   ![FCD Proof](/assests/images/FCD Proof.png "FCD Proof")
2. Cycle's Starting Point Detection

