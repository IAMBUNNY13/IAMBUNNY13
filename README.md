import subprocess

s = subprocess

def Game():


  s.call(["say", "Hello welcome to trivia"])
  print("Hello welcome to trivia")

  
  s.call(["say", "Are you ready to start YES/NO"])
  ans = input("Are you ready to start YES/NO: ")
  

  

  Q = 3
  QCorrect = 0

  if ans.lower() == 'no':
    s.call(["say", "Okay goodbye"])
    print("Okay goodbye")
    

  if ans.lower() == 'yes':
    s.call(["say", "What is 1+1: "])
    ans = input("What is 1+1: ")
    
    
    if ans.lower() == '2':
      QCorrect += 1



    s.call(["say", "What is 96x96: "])
    ans = input("What is 96x96: ")
   
      
    if ans.lower() == '9216':

      QCorrect += 1
        


    s.call(["say", "What is the best color: "])
    ans = input("What is the best color: ")
    
      
    if ans.lower() == "blue":
      QCorrect += 1

    


    mark = (QCorrect/Q) * 100

        

    
    
    print("Precent:", int(mark))
    s.call(["say", "Do you want to try again? YES/NO: "])
    ans = input("Do you want to try again? YES/NO: ")
   
    
    
    if ans.lower() == 'yes':
      print("Okay")
      Game()
    else:
      print("Okay Bye")
      
Game()
  
      
      
      
    
    
    




    
