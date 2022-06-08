def push(a,data):
    a.append(data)
    print("ELEMNT PUSHED SUCCESSFULLY ")
def pop(a):
    x=a.pop()
    print("ELEMENT POPED SUCCESSFULLY ")
def peek(a):
    print("ELEMENT  PEEKED SUCCESSFULLY ")
def displayall(a):
    for i in range(len(a) -1,-1,-1):
        print(a[i])
        print("ELEMENT DISPLAY ALL SUCCESSFULLY")

    

#--main--
a=[]
while True:
    choice = int(input(" 1->push \n 2->pop \n 3->peek \n 4->display all \n 5->exit \n enter your choice ::"))
    if choice == 1:
        data=int(input("ENTER VALUE TO BE PUSHED ::"))
        push(a,data)
    elif choice == 2:
        if len(a) == 0:
            print("STACK UNDERFLOW")
        else:
            pop(a)
            
    elif choice == 3:
        if len(a) == 0:
            print("STACK UNDERFLOW")
        else:
            peek(a)
            
    elif choice == 4:
        if len(a) == 0:
            print("STACK UNDERFLOW")
            
        else:
            displayall(a)
            
    elif choice ==5:
        break
    
    else:
        print("ELEMENT SHOULD BE FROM 1 TO 5")
    
