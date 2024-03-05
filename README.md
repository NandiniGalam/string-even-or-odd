# string-even-or-odd
#string 
s=input()
x=s[::2]
print(len(x))


#spearating even odd
#approach2
s=input()
x=[]
for i in range(len(s)):
  if i%2==0:
    x.append(s[i])
y=[]  
for i in range(len(s)):
  if i%2!=0:
    y.append(s[i])
x.extend(y)
print(*x,sep="")

#approach 3
s=input()
x=""
y=""
for i in range(len(s)):
  if i%2==0:
    x=x+s[i]
for i in range(len(s)):
  if i%2!=0:
    y=y+s[i]
print(x+y)    
