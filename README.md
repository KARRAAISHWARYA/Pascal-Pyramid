# Pascal-Pyramid


N = int(input())
 
nums = list(map(int,input().split()))
 
nums.sort()
 
shortlist = nums[-6:]
 
a = shortlist[0]
f = shortlist[1]
c = shortlist[-1]
d = shortlist[-2]
e = shortlist[-3]
b = shortlist[-4]
 
result1 = sum([a,4*b,6*c,4*d,e])
result2 = sum([f,4*b,6*c,4*d,e])
 
result11 = result1*sum([b,4*c,6*d,4*e,f])
result22 = result2*sum([b,4*c,6*d,4*e,a])
print(max(result11,result22))


