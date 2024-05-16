# LEET-CODE
# Python (Leetcode problems on Top Interview 150 )
class Solution:
    def isPalindrome(self, x: int) -> bool:
        rev = 0
        copy = x
        if (x<0):
            return False
        #return True
        while x!=0:
            rev = (rev*10)+ (x%10)
            x//=10
        if rev == copy:
            return True
        return False        
