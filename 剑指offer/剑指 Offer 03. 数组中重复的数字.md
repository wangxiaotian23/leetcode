#### [剑指 Offer 03. 数组中重复的数字](https://leetcode-cn.com/problems/shu-zu-zhong-zhong-fu-de-shu-zi-lcof/)

```java
class Solution {
    public int findRepeatNumber(int[] nums) {
        int arr[]=new int[nums.length];
        for (int i = 0; i <nums.length ; i++) {
            arr[nums[i]]++;
            if (arr[nums[i]]>1){
                return nums[i];
            }
        }
        return -1;
    }
}
```

