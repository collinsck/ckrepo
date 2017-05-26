# ckrepo
shutdown = False

balance = float( 150000)

format (balance, '.2f')



def printbalance ():
    '''this prints the Balance to the user'''
    return (balance)
    


        

def deposit ():
    '''This adds the user inputted float to the balance'''
    global balance
    deposited = float(input("How much would you like to deposit today?: "))
    if deposited > (15000):
        print ("That's not a valid amount.")
    else:
    	balance += deposited
    	print ("Deposit complete. Balance updated")
	
        
       

def withdrawbalance ():
    '''This function withdraws funds from the user's account balance. If the balance is too low, it returns an error.'''
    
    withdraw = int(input("What amount do u need: "))
    if withdraw > (50000):
        print ("error")
        
    else:
	        
          print ("balance-=deposited")
    	    

    

while (shutdown == False):
#added in to keep refreshing the menu after an action is made/input is made


    
    print (" ")
    print ("menu")
    print (".............. ")
    print ("1 = Make a deposit")
    print ("2 = Make a withdrawal")
    print ("3 = view balance")
    print ("4 = quit program")
    userchoice = int(input ("What would you like to do?: "))

    if (userchoice ==1):
        deposit ()
        
        
    elif (userchoice ==2):
        withdrawbalance ()
		
		
		
       
            
    elif (userchoice ==3):
        printbalance ()
        print ("Your current balance: ")
        print (balance)


   
        
    elif (userchoice ==4):
        print ("Thank you for banking with us")
        quit

        shutdown = True

    else:
        print ("Error")


