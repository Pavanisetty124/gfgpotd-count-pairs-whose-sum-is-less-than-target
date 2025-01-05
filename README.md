# gfgpotd-count-pairs-whose-sum-is-less-than-target
class Solution:
    #Complete the below function
    def countPairs(self, arr, target):
        #Your code here
        arr.sort()
        left=0
        right=len(arr)-1
        count=0
        while left<right:
            if arr[left]+arr[right]<target:
                count+=(right-left)
                left+=1
            else:
                right-=1
        return count


//this is the two-pointer aprroach 
time-complexity:o(nlogn)
space-complexity:o(1)


class Solution:
    #Complete the below function
    def countPairs(self, arr, target):
        #Your code here
        arr.sort()
        n=len(arr)-1
        for i in range(n):
            for j in range(i+1,n):
                 if arr[i]+arr[j]<target:
                count+=1
        return count

      //this is the brute force approch 
      time-complexities:o(n^2)
      space-complexity:o(1)
      
             
        
