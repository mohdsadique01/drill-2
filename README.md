pipes
question 1

Download the contents of "Harry Potter and the Goblet of fire" using the command line from

answer 
wget https://raw.githubusercontent.com/bobdeng/owlreader/master/ERead/assets/books/Harry%20Potter%20and%20the%20Goblet%20of%20Fire.txt
mv "Harry Potter and the Goblet of Fire.txt" harry


quwstion 2

Print the first three lines in the book through commmand

answer 2
cat harry | head -3


question 3 

print the last 10 line number through command

asnwer 3
cat harry | tail -10

question 4

How many times do the following words occur in the book through command line
FOR Harry word

answer 4 (a)
grep -o -i Harry harry | wc -l

for Ron
answer 4(b)
grep -o - i ron harry | wc -l
 
 for hermione
 answer 4 (c)
 grep -o -i hermione harry | wc -l

for dumbledore
answer 4 (d)
grep -o -i dumbledore harry | wc -l



question 5

Print lines from 100 through 200 in the book through command line

answer 5

sad -n -e "100,200" harry


question 6

How many unique words are present in the book through command line

answer 6

cat harry|tr '\n' ' '|tr '\t' ' '|tr -s ' '|tr ' ' '\n'|sort|uniq|wc




Processes, ports

question 1

List your browser's process ids (pid) 


parent process ids(ppid) through command


answer 1
 
ps -o ppid= -p 9801

question 2

Stop the browser application from the command line if i am using from firefox then

answer 2 

ps -ax | grep firefox

question 3

List the top 3 processes by CPU usage by using command

answer 3

ps aux --sort -%cpu | head -3


question 4

List the top 3 processes by memory usage.

answer 4

ps aux --sort -%mem | head -3


question 5

Start a Python HTTP server on port 8000 by command line

answer 5

python -m SimpleHTTPServer 8000

quesstion 6

Open another tab. Stop the process you started in the previous step

answer 6

kill $(pidof ping)


question 7

Start a Python HTTP server on port 90 through command line

answer 7
python -m SimpleHTTPServer 90

question 8
Display all active connections and the corresponding TCP / UDP ports.


answer 8

netstat -at
netstat -au
  

question 9

Find the pid of the process that is listening on port 5432

first of all install net tools to find process of listning port command is

answer

sudo get.apt install net-tools

after that finding procees of port then command is 
lsof -i :5432
then find the process name using PID number with the ps command like so
$ ps -p 5432 -o comm=





Managing software
question 1

for Installing htop, vim and nginx

answer 1

sudo apt install htop
sudo apt install vim
sudo apt install nginx

question 2

for Uninstall nginx and command is

answer 2

sudo apt purge nginx





MISC


question 1

What's your local IP address and command is

answer 1

hostname , ifconfig , or ip commands


question 2

Find the IP address of google.com

answer 2

host gooogle.com

qwuestio 3

How to check if Internet is working using CLI?

answer 3

ping -c 3 google.com

question 4

Where is the node command located? What about code?
# Answer 4)a) node commmand is located in bin file.
  whereis node
  
 b)
  whereis code
 code: /snap/bin/code
