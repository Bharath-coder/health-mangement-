def getdate():
    import datetime
    return datetime.datetime.now()

t =getdate()
#print(str(t))
def log(k):
    if k==1 :
        i =int(input("1 for exercise 2 for food"))
        if i ==1:
            inp =input("enter a value ")
            with open("harry_ex","a") as f:
                f.write (str(t) +":" +inp +"\n") 
            print("want to try again")
           
        else:
            inp =input("enter a value \n")
            with open("harry_f","a") as f:
                f.write(str(t) +":" +inp+"\n")
            print("want to try again")

    elif k==2 :
        i =int(input("1 for exercise 2 for food"))
        if i ==1:
            inp =input("enter a value\n" +"\n")
            with open("johny_ex","a") as f:
                f.write (str(t) +":" +inp+"\n")
            print("want to try again")

        elif i==2:
            inp =input("enter a value \n"+"\n")
            with open("johny_f","a") as f:
                f.write(str(t) +":" +inp +"\n")
            print("want to try again")

    elif k==3 :
        i =int(input("1 for exercise 2 for food"))
        if i ==1:
            inp =input("enter a value \n")
            with open("bonnie_ex","a") as f:
                f.write (str(t) +":" +inp +"\n")
                
            print("want to try again")
            
        else:
            inp =input("enter a value")
            with open("bonnie_f","a") as f:
                f.write(str(t) +":" +inp +"\n")
            print("want to try again")


    
def retrieve(k):
      if b==1 :
        i =int(input("1 for exercise 2 for food "))
        if i ==1:
            with open("harry_ex") as f:
                print(f.read())

        else:
            with open("harry_f") as f:
                print(f.read())

      if b==2 :
        i =int(input("1 for exercise 2 for food "))
        if i ==1:
            with open("johny_ex") as f:
                print(f.read())

        else:
            with open("johny_f") as f:
                print(f.read())
      if b==3 :
        i =int(input("1 for exercise 2 for food "))
        if i ==1:
            with open("bonnie_ex") as f:
                print(f.read())

        else:
            with open("bonnie_f") as f:
                print(f.read())
      
while(True):
  i =input("enter y to try")
  if(i =="y"):
   a =int(input("1 for log 2 for retrieve"))
   if a ==1 :
         b =int(input("1 for harry 2 for jhony 3 for bonnie "))
         log(b)

   else:
    
    b =int(input("1 for harry 2 for jhony 3 for bonnie "))
    retrieve(b)
  else:   
     print("thank you \n ")
     break
    



