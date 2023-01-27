INSTALLING VS CODE
<img width="1200" alt="Screenshot_20230111_034153" src="https://user-images.githubusercontent.com/122497642/212381254-1a12e71a-9f73-4973-9aa2-2890d09157c2.png">

While I skipped the step to install VScode on my laptop, since I already had it, it can be downloaded through the VScode website. Depending on if the user's operating system is a macOS or Windows, the correct version must be downloaded for the corresponding device. Once downloaded, the image above should appear when VScode is opened.


REMOTELY CONNECTING
<img width="1000" alt="Screenshot_20230111_040615" src="https://user-images.githubusercontent.com/122497642/212381257-e3ff3ea7-9b26-4b36-9344-2bf340be589f.png">

After installing git, I set the default terminal to use git bash. Then a new terminal was opened and I typed in ssh and my course-specified acount as a command, which prompted the server to ensure that I wanted to continue connecting since it's a new server, and then entered my password. The terminal is now connected to the server when the screen in the above image shows up.


TRYING COMMANDS
<img width="1000" alt="Screenshot_20230111_041441" src="https://user-images.githubusercontent.com/122497642/212381259-d7c5e092-7e81-4a60-8add-379ebccbaf6e.png">

Once connected to the server, I tested out some commands including cd ~, cd, ls -lat, ls -a, ls directory where directory is /home/linux/ieng6/cs15lwi23/course-specified username, cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/, cat /home/linux/ieng6/cs15lwi23/public/hello.txt. The last two commands produced an error since hello.txt didn't exist and so did the ls directory command. The other commands seemed to work properly and then I logged out using ctrl + D. ls directory lists all the folders and files in that directory. ls -lat shows all the contents in the directory in a long-list format. ls -a lists all the files, including the hidden ones. cd ~ allows you to go to the root home directory. cp directory copies files from one location to another. cat directory prints contents of a file given by the directory.
