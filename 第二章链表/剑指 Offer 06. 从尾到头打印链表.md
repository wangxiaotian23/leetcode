#### [剑指 Offer 06. 从尾到头打印链表](https://leetcode-cn.com/problems/cong-wei-dao-tou-da-yin-lian-biao-lcof/)

```java
class Solution {
    public int[] reversePrint(ListNode head) {
       Stack<Integer> stack=new Stack<Integer>();
        ArrayList<Integer> list=new ArrayList<Integer>();
        while (head!=null){
            stack.push(head.val);
            head=head.next;
        }
        while (!stack.isEmpty()){
            int x=stack.pop();
            list.add(x);
        }
        int [] arr=new int[list.size()];
        for (int i = 0; i <list.size() ; i++) {
            arr[i]=list.get(i);
        }
        return arr; 
    }
}
```

