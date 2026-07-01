Day11-Bashing for Beginners

Bash stand for Bourne Again Shell

Command

which $SHELL to find which type of script you want to run python bash or etc
 
echo Write inside the file content

nano Editior for linux

For Bashing

#!/bin/bash
This is the first line in every script we need.

Example

Terminal: $nano hello.sh

We will go insdie the hello.sh editor

#!/bin/bash

echo   “Hi ubantu”
echo Today is: $(date)

cntrl + x then y and hit the enter 

then we have to give it the execute file command 

$ chmod +x hello.sh

Then after we will execute the $ bash hello.sh

The output will be 

Hello ubantu
Today= current date 




Variables
It lets us store value and reuse throughout the your script and , bash variabels has no types.

Assigning Variables
Assign a value with = sign there must be not space around the sign

Example
Terminal: $nano hello.sh

We will go insdie the hello.sh text editor

#!/bin/bash

name=rayan

echo “Good morning $name”
Sleep 1
echo “You’re  looking  good today $name”
sleep 1
echo “You have the best hairstyle $name,I’ve ever seen”

cntrl + x then y and hit the enter 

Then after we will execute the $ bash hello.sh

The output will be 

Good morning Rayan
Adter 1s
You’re  looking  good today rayan
After 1s
You have the best hairstyle $name,I’ve ever seen

Or we can do
 
echo “What is you name”

read name 

then output will be 

What is you name 
-Dipen
Then output will be your name this help people to run the script with their name no problem
Special Variables

-$1,$2 the first,second arguments passed to scipt also called positional argument]

Terminal: $nano hello.sh

We will go insdie the hello.sh text editor

#!/bin/bash

name=$1
compliment=$2

echo “Good morning $name”
Sleep 1
echo “You’re  looking  good today $name”
sleep 1
echo “You have the best $compliment $name,I’ve ever seen”

cntrl + x then y and hit the enter 

Then after we will execute the $ bash hello.sh Dipen Eyes

The output will be 

Good morning Dipe 
Adter 1s
You’re  looking  good today  Dipen
After 1s
You have the best Eyes Dipen I’ve ever seen














Example 

Terminal: $nano hello.sh

We will go insdie the hello.sh text editor

#!/bin/bash

name=$1
compliment=$2

directory=$(pwd)
user=$(whoami)
date=$(date)

echo “Good morning $name”
Sleep 1
echo “You’re  looking  good today $name”
sleep 1
echo “You have the best $compliment $name,I’ve ever seen”
sleep1

echo “You are logged in as $user and I m at this $directory.Today is: $date”

cntrl + x then y and hit the enter 

Then after we will execute the $ bash hello.sh Dipen Eyes

The output will be 

Good morning Dipe 
Adter 1s
You’re  looking  good today  Dipen
After 1s
You have the best Eyes Dipen I’ve ever seen


You are logged in as username and I m at this directory.Today is date current date
<img width="468" height="645" alt="image" src="https://github.com/user-attachments/assets/394d040a-63a4-4116-8770-31f7a1d8aca6" />
