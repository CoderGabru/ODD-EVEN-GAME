# ODD-EVEN-GAME
 # playagain = True # while playagain == True: class gameplay:       def youbatting(self):           t = True           self.yruns = 0           while (t == True):                shot = int(input("IT'S YOUR TURN INTER THE NUMBER HERE: "))            delivery = random.randint(1,10)            print(f"COMP CHOOSE: {delivery}")                        if(delivery!=shot ):              self.yruns = self.yruns + shot              t= True               else:              t = False              print("**** OUT ****")                print(f"YOUR SCORE IS:  {self.yruns}")                             def compbatting(self):              t = True             self.cruns = 0             while(t== True):               delivery = int(input("ITS YOUR TURN ENTER THE NUMBER HERE: "))               shot = random.randint(1,10)               print(f"COMP CHOOSE: {shot}")               if (delivery != shot):                   self.cruns = self.cruns + shot                   t = True               else:                   t= False                   print("**** CLEAN BOWLED ****")                   print(f"COMPUTER SCORE IS: {self.cruns}")                                           def result(self):                      if( self.yruns&lt;self.cruns):               print("**** YOU LOOSE THE GAME..... BETTER LUCK NEXT TIME ****")            else:               print("**** CONGRATULATIONS....YOU HAVE WON THE GAME")                     player = gameplay()  #TOSS import random import typing  print("**************   WELCOME TO ODD EVEN GAME CREATED BY RAGHAV   **************") print("*****INSTRUCTION***** ......ALWAYS USE NUMERS FROM 1 TO 10") print( "***** TOSS *****        ") you =input("ODD(o) OR EVEN(e): ")  tossvalue = int(input("YOUR TURN: "))#.........you chosses value for toss compchoose = random.randint(1,10) #.........computer chooses value for toss print("computer choose: ", compchoose)  if(you=="e"):        if (tossvalue+compchoose)%2==0:            toss = True            print("YOU WON THE TOSS")        else:            toss = False            print("YOU LOSS THE TOSS") elif(you == "o"):      if(tossvalue+compchoose)%2==0:          toss = False          print("YOU LOOSE THE TOSS")      else:          toss = True          print("YOU WON THE TOSS") #if you won the toss  if toss == True:     you_batball = input("BATTING(ba) OR BOWLING(bo): ") #you choose batting or bowling     #IF YOU CHOOSE BATTING     if you_batball == "ba":        player.youbatting()      print("NOW IT'S YOUR BOWLING ")       player.compbatting()      player.result()      else:         player.compbatting()         print("NOW IT'S YOUR BATTING ")         player.youbatting()         player.result()     #if comp won the toss  else:  comp_batball = random.randint(1,2) #comp choose batting or bowling  if(comp_batball== 1):        # if computer choose batting             print("computer choose Batting" )             player.compbatting()             print("NOW IT'S YOUR BATTNG ")             player.youbatting()             player.result()                else:                          # if computer choose bowling             print("computer choose bowling")             player.youbatting()             print("NOW IT'S YOUR BOWLING ")             player.compbatting()             player.result()   endline = input("**** DO YOU WANT TO PLAY AGAIN....YES(y) OR NO(n) ****")  # if( endline == "y"): #     playagain = True # else: #     playagain =False
