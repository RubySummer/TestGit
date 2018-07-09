#public class Solution {
##public static void main(String[] args) {
###ListNode l1 = new ListNode(2);
###l1.next = new ListNode(4);
###l1.next.next = new ListNode(6);
###ListNode l2 = new ListNode(5);
###l2.next = new ListNode(6);
###l2.next.next = new ListNode(4);
###ListNode node = addTwoNumbers(l1,l2);
###while(node!=null) {
####System.out.println(node.val);
####node = node.next;
###}
##}
##public static ListNode addTwoNumbers(ListNode l1, ListNode l2) {
###ListNode temp = new ListNode(0);
###ListNode p=l1,q=l2, current= temp;
###int num1=0,a=0,b=0;
###while(p!=null||q!=null) {
####if(p!=null) {
#####num1+=p.val;
#####p=p.next;
####}
####if(q!=null) {
#####num1+=q.val;
#####q=q.next;
####}
####a = num1%10;
####b = num1/10;
####num1 = b;
####current.next=new ListNode(a);
####current=current.next;
###}
###if(b==1) {
####current.next = new ListNode(1);
###}
###return temp.next;
##}
#}
