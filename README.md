items=["1","2","3","4","5","6","7","8","9",]
itf=input()
found=False
first=0
last=len(items)-1
while found==False and last>first:
    midpoint=(first+last)//2
    if items[midpoint]==itf:
        found=True
    else:
        if items[midpoint]<itf:
            first=first+1
        else:
            last=last-1
if found==True:
    print("item found at",midpoint)
else:
    print("item not found")
