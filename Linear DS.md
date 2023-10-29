# Notes
- https://leetcode.com/problems/remove-nth-node-from-end-of-list
- https://leetcode.com/problems/odd-even-linked-list/
- https://leetcode.com/problems/merge-k-sorted-lists/

# Linked List

## Algorithms
1. Floyd Cycle Detection (FCD)<br>
   1. slow = slow -> next, fast = fast->next->next
   2. if(slow == fast) "cycle" else (fast == null) "no cycle"<br>
   > ![FCD Proof](/assests/images/fcd-proof.png "FCD Proof")
2. Cycle's Starting Point Detection
   1. p1 = head, p2 = slow // fast meeting point
   2. p1 = p1->next p2 = p2->next
   3. if(p1 == p2) return p1 // starting point
   > Proof
   > ![FCD Proof](/assests/images/fcd-proof-ii.png "FCD Proof 2")

# Stack

## Algorithms
1. Next Greater Elememt(NGE)
   - Invariant ? Invariant is the property (part of the program) of stack that remains constant throughout the runtime of the algorithm.
   - In this(NGE) case
     - Monotonus Stack (Always decreasing)
     - Elements in stack are always the ones for which NGE has to be determined.
2. NGEII
   - Problem - https://leetcode.com/problems/next-greater-element-ii/
   - Since it is a circular list, we can loop the array twice.
   - `for(i = 0; i < 2*size; i++){currIdx = i%2;}`
   - This will convert the array into a1,a2,...an,a1,a2,....an.
