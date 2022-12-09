# python-1
x=int(input("Enter starting number: "))
y=int(input("Enter end number: "))
if x>0 and y>0:
    print()
    print()
    a=0
    b=0
    if x==1:
        print("1 is nor prime nor composite number")
        x=x+1

    for i in range(x,y+1):
        for j in range(2,i):
            if i%j==0:
                a=a+1
                print(i,"is composite")
                break
        else:
            b=b+1
            print(i,"is Prime")
    print()
    print(f"There are {a} composite numbers and {b} prime numbers in given range.")
else:
    print("Enter only positive integers")
