# Print-Reverse-LinkedList
You have been given a singly linked list of integers. Write a function to print the list in a reverse order. To explain it further, you need to start printing the data from the tail and move towards the head of the list, printing the head data at the end.
//answer
public class Solution {

	public static void printReverse(LinkedListNode<Integer> root) {
					if(root==null) {// base case
			return ;
		}
		//System.out.println(head.data);
		printReverse(root.next);
		System.out.print(root.data+" ");
	}

}
