## Solution     
The first thing that came into my mind was to google up the name Kadour Tan, yet i found nothing intresting.   
So I thought why not search the name in github :   
lesgoo we found a user:        

![image](https://github.com/user-attachments/assets/175259a9-0bb2-43c5-a9dc-50571687c8c4)        
    
Let's check out his account : [repo link ](https://github.com/kadourtan)    
     
There are 4 repos : 
- a repo with a weird encrypted name that seems like base64 : **"aGludHM"** when decoding it with cybercheff from base64 we get the word **"hints"**, it has a txt file with the name something_you_wouldnt_like.txt which contains some quotes amongst them :
> "what looks like a simple string could be the missing piece of the puzzle." and "Sometimes, data is hidden where you least expect it—like". lets move on and see maybe those quotes will come in handy.       
- another repo with an encrypted base64 name :**"YmFja2Rvb3I"** which when decoding reads as **"backdoor"**. movin on
- a repo named bit-l93ad it has a zipped file in it named work. I downloaded it but i couldnt open it : it needs a password
- a repo named private configs with a python script named security tools : the scrupt prompts the user into entering a password then hashes it into sha256. It also stores a weird encrypted string into a variable named **hidden_passphrase** 
  when decoding it we get the word **"fake_password"**. it's clearly there to throw us off.
  Lets look somewhere else. I noticed the repo has a previous commit : lets check it out
  It contains a similair code however another encrypted word is getting stored into the **hidden_passphrase** variable. when decoding it we got : **"passtan"**
  Lets try and put it into the zipped file.
     
LESSGOO WE GOT IN
      
It contains a secret.txt file which appears to be a security incident log, specifically an SSH intrusion log, however there is something that cought my eye :
  > [2025-02-12 03:18:40] command: touch -.-- --- ..- .----. .-. . ..--.- ... --- ..--.- -.-. .-.. --- ... . ..--.- -.- . . .--. ..--.- .-.. --- --- -.- .. -. --. ..--.- .... . .-. . .-.-.- .-.-.- .-.-.-
  > 
It looks like morse code. lets decode it using cybercheff:            
      
![image](https://github.com/user-attachments/assets/d0571038-9531-4a4b-80eb-548f38473025)
       
Lets keep looking. oh look another one :
  >    [2025-02-12 03:45:12] command: echo"-- .. -.-. .-. --- -.-. - ..-.  -.-- ----- ..- ..--.- -.. .---- -.. ..--.- ....- ..--.- --. .-. ...-- ....- --... ..--.- .--- ----- ---.. ..--.- ..... --... ....- .-.. -.- .---- -. --. ..--.- -- ...-- " > /dev/null       
                    
and when decoding it we get :            
   
![image](https://github.com/user-attachments/assets/c8022e5d-ae01-461e-a5a1-a444b641c59e)

**WHICH PRETTY MUCH LOOKS LIKE THE FLAGG**


