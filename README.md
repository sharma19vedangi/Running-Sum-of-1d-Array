# Running-Sum-of-1d-Array
#Array Leetcode Problem Solution
class Solution {
    public int[] runningSum(int[] nums) {
        int a[]=new int[nums.length];
        a[0]=nums[0];
        int sum=a[0];
        for(int i=1;i<nums.length;i++)
        {
            a[i]=nums[i]+sum;
            sum=a[i];
        }
        return a;
    }
}
