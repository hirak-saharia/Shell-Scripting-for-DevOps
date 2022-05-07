# Shell-Scripting-for-DevOps

Let's assume we have multiple if else condition:
 
  We have three variable like
     
      a = 100
      b = 200
      c = 300
  So, how to find the greatest number from the above variable?
  
  
    Sol: nano if_else.sh
    
         #!bin/bash
    
         
         if [[ $a -gt $b && $a -gt $c ]]
    
         then
         
         echo "A is the greatest"
         
         elif [[ $b -gt $a && $b -gt $c ]]
       
         then
         
         echo "B is the greatest"
         
         else 
         
         echo "C is the greatest"
         
         fi
         
         save the script and execute
         
         chmod 777 if_elif.sh
        
         ./if_elif.sh
         bigger
   
   Let's explore Loops in Shell scripting - Let's print 1 to 10 numbers
   
        nano loops.sh
        
        #!/bin/bash
        
         for ((i=0; i<10; i++))
         
         do
         
         echo "$i"
         
         done
  
  Let's explore some advance workflow .....
  
  Let's iterate files using loops
         
         Let's create a file 
         
         touch file_1.text
         
         touch file_2{2..10}.txt     #it means in short till 10 files will be created from second file
         
   Now let's Iterate 10 files using for loop function
   
         #!/bin/bash
         
         for ((i=0; i<10; i++))
         
         do
         
         echo "$i"
         
         done
         
         for FILE in *.txt
         
         do
         
         echo $FILE
         
         done
         
