#Basic Program that analyses if your name is retarded

print ('Hello User!')
print ('This program analyses if you are a retard by simply looking at your name!')
print ('Please enter your name:')

counter = 1
while counter <5:
    UserName = input()
    UserName_Count = len(UserName) #Calculate number of letters in name)

#UserName_Count check
    
    if UserName_Count==0:
        print ('sorry please enter a name:')
        
    elif UserName_Count>=1:
        
        Values=[]

        import random  #Generate 15 random numbers from 1 to 25, comparing with username length
        from random import randint

        for x in range(15): 
            Values.append(random.randint(1,25))
    
        if UserName_Count in Values:
            print ('sorry you are retarded')
        else: print  ('Congratulations! You are likely not retarded!')
    
        print ('Please enter another name:')
