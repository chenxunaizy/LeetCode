"""
LeetCode
#1.TwoSum
Description:Given an array(List) and a target,return indices of two numbers  that add up to a specific target
Solution:
Method:
add 160524
"""
"""
"""
class Solution:
    def __init__(self):
        self.resLessThanHalf=[]
        self.resMoreThanHalf=[]
        self.finalRes=[]
    def twoSum(self,lists,target):

        """
        :param arr:List[int]
        :param target:int
        :return:List[int]
        """
        if(lists.count(target/2)>1):
            targetHalf=target/2
            for (i,x) in enumerate(lists):
                if(x == targetHalf):
                    self.finalRes.append(i)
        else:
            for (i,x) in enumerate(lists):
                if(x < target/2):
                    self.resLessThanHalf.append(x)
                else:
                    self.resMoreThanHalf.append(x)
            for x in self.resLessThanHalf:
                y = target-x
                if( self.resMoreThanHalf.count(y)):
                    self.finalRes.append(lists.index(x))
                    self.finalRes.append(lists.index(y))
        if(len(self.finalRes)>1):
            return self.finalRes
        else:
            return "No matching numbers"
