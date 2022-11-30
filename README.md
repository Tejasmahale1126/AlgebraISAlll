# AlgebraISAlll
print("ENTER 1: FOR ORDER OF ELEMENTS OF Zn ")
print("ENTER 2: FOR GENERATORS OF Zn ")
c=int(input("Your Choice "))
if c==1 :
	n= int(input("Enter your choice of n for Zn "))
	set=list(range(n))
	print("Your set is:")
	print("Zn ="+str(set))
	a=0
	for j in range(1,20,1):
			s= int(input("I want the order of "))
			if s==0 :
				print("Order of 0 is 1")
			elif s>0 and s<n :
					t=0
					for i in range(1,s+1,1):
						if s%i==0 and n%i==0 :
							gcd=i
					a=int(n/gcd)
					print("Order of "+str(s)+" by formula is "+str(a)+" ")
					for i in range(1,n+1,1):
					    t=(s+t)%n
					    if t%n==0 :
					     print("Order of "+str(s)+" by search method is "+str(i)+" ")
					     break
			else :
			     print("INCORRECT ENTRY!!!!")
			     print("PLEASE CHOOSE AN ELEMENT FROM THE SET!!!!")
		     
if c==2 :
	for j in range(1,20,1):
		n= int(input("Enter your choice of n for Zn "))
		set=list(range(n))
		print("Your set is: ")
		print("Zn ="+str(set))
		print("The Generators of Zn are:")
		for k in range(1,n,1):
			gcd=0
			for i in range(1 ,k+1,1):
			  	 if n%i==0 and k%i==0 :
			  	 	gcd=i
			if gcd==1 :
				print(" "+str(k)+" ") 
