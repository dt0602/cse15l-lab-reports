## Step 4

<img width="750" alt="image" src="https://user-images.githubusercontent.com/122497642/221689452-4212ee50-1cc7-4a84-b29b-3b72406ffbd7.png">

To get `ssh cs1lwi23aoq@ieng6.ucsd.edu`, I used `<ctrl-R>` and typed in `s` to get the rest of the line. After that, I just had to type in my password to log into my ieng6 account.

## Step 5

<img width="750" alt="image" src="https://user-images.githubusercontent.com/122497642/221689644-12d4b32b-0429-4057-b988-21b42322982b.png">

I forked this repository from the lab document to my account and opened Github Desktop to clone the repository. Then I copied the url of the forked repository. After ssh'ing into the ieng6 account, I typed `git clone` and pasted the url and hit `<enter>` to clone the directory into the ieng6 account. I entered `cd lab7` to get inside the directory.

## Step 6

<img width="750" alt="image" src="https://user-images.githubusercontent.com/122497642/221689842-05010f4a-82f9-4e15-b19c-9affa3342ea5.png">

To run the tests I used `<ctrl-r>` and typed in `j` to find the compile command `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` and the run command `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore`, where I added `ListExamplesTests`. 

## Step 7

<img width="750" alt="image" src="https://user-images.githubusercontent.com/122497642/221689947-de7b0a98-09be-4a58-90a3-9d6cfb7019c5.png">
<img width="750" alt="image" src="https://user-images.githubusercontent.com/122497642/221690088-33ce811b-40f2-4e41-aa9d-e434d88399db.png">

To edit the file to fix the errors, I entered `nano ListExamples.java` to directly access the program. In the last while loop of the code, I changed `index1 += 1` to `index2 += 1` because the error was that the wrong index variable was incremented, creating and endless while loop. I hit `<ctrl-o>`and `<enter>` tosave the file and `<ctrl-x>` to exit out of the editing file.

### Step 8

<img width="750" alt="image" src="https://user-images.githubusercontent.com/122497642/221690178-08aafa7a-481c-445a-83a5-e87510112baf.png">

To test the file again, I hit `<up><up><up><enter>` and `<up><up><up><enter>` to compile and run the test file with no errors this time. 

### Step 9

<img width="750" alt="image" src="https://user-images.githubusercontent.com/122497642/221696261-2b224a5c-8416-4f46-9819-4581c6368277.png">
<img width="750" alt="image" src="https://user-images.githubusercontent.com/122497642/221696312-3dda0770-f640-4cd2-84a0-286032c7b116.png">

Finally I needed to commit and push these changes to my Github account. To do so, I first used the command `git add L<tab>`, where I got `git add ListExamples` and the options `ListExamples.java` and `ListExamples.class`. I then typed in `git add L<tab>.java`, since `ListExamples.java` was the file I changed. Then to commit, I typed in `git commit -m "Changes"`. To push these changes, I had to enter in the command `git push`, where it prompted me to type in my github username and password. 
