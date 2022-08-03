pipes
question 1

Download the contents of "Harry Potter and the Goblet of fire" using the command line from
first of all we have to install curl
sudo apt install curl
after that to download file through url command is
curl -o[url]
after that to save the file throgh command
curl-o [filename] [url]

quwstion 2
Print the first three lines in the book through commmand
head -n1 [harry]
head -n2 [harry]
head -n3 [harry]


question 3 
print the last 10 line number through command
tail -n10 harry

question 4

How many times do the following words occur in the book through command line
FOR Harry word
grep -o -l Harry harry | wc -l

for Ron
grep -o -l ron harry | wc -l
 
 for hermione
 grep -o -l hermione harry | wc -l

for dumbledore
grep -o -l dumbledore harry | wc -l



question 5

Print lines from 100 through 200 in the book through command line
sad -n -e "100,200" harry


question 6
How many unique words are present in the book through command line
cat harry|tr '\n' ' '|tr '\t' ' '|tr -s ' '|tr ' ' '\n'|sort|uniq|wc




Processes, ports

question 1

List your browser's process ids (pid) 


parent process ids(ppid) through command

ps -o ppid= -p 9801

question 2

