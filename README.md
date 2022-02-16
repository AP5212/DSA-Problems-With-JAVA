# DSA-Problems-With-JAVA
66. Plus One Leetcode problem solution in java
https://leetcode.com/problems/plus-one/

class Solution {
    public int[] plusOne(int[] digits) {
        int idx = digits.length - 1;
        int[] ans = new int[digits.length + 1];
        
        while(idx >= 0){
            if(digits[idx] == 9){
                digits[idx] = 0;
            }else{
                digits[idx] += 1;
                return digits;
            }
            idx--;
        }
        
        ans[0] = 1;
        return ans;

    }
}
