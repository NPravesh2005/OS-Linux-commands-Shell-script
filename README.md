# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
<img width="494" height="245" alt="Screenshot 2025-08-13 110201" src="https://github.com/user-attachments/assets/c645ebb6-4426-41f2-b037-f3979f5cd1e7" />


cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```

<img width="532" height="282" alt="Screenshot 2025-08-13 110248" src="https://github.com/user-attachments/assets/3765e3f2-6e75-479c-8339-21b5f0c4b496" />

### Display the content of the files
cat < file1
## OUTPUT

<img width="507" height="238" alt="Screenshot 2025-08-13 110504" src="https://github.com/user-attachments/assets/cbb72396-75b5-44c8-a982-bd66f3e5912c" />


cat < file2
## OUTPUT
<img width="524" height="293" alt="Screenshot 2025-08-13 110525" src="https://github.com/user-attachments/assets/1bec37ab-1a05-4f85-ab84-6429cf64ced5" />


# Comparing Files
cmp file1 file2
## OUTPUT
 <img width="643" height="127" alt="Screenshot 2025-08-13 110553" src="https://github.com/user-attachments/assets/e3392666-85a8-4c0e-ab79-72dbe45712e7" />

comm file1 file2
 ## OUTPUT
<img width="593" height="371" alt="Screenshot 2025-08-13 110635" src="https://github.com/user-attachments/assets/3f7af970-957c-4f2d-ac33-31ad5f46c7ec" />

 
diff file1 file2
## OUTPUT
<img width="586" height="454" alt="Screenshot 2025-08-13 110701" src="https://github.com/user-attachments/assets/2fc744c5-5561-4b3d-b8eb-420f8009a49c" />


#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
<img width="579" height="164" alt="Screenshot 2025-08-13 110747" src="https://github.com/user-attachments/assets/b9434f6f-e5ee-42c1-b35a-4565f2f83e83" />


cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```

<img width="585" height="209" alt="Screenshot 2025-08-13 110829" src="https://github.com/user-attachments/assets/f98672eb-71c0-47d3-80d2-843c2aec2677" />

cut -c1-3 file11
## OUTPUT

<img width="509" height="162" alt="Screenshot 2025-08-13 110912" src="https://github.com/user-attachments/assets/39931aa1-ca12-45d9-9ebd-e29692ef5ead" />



cut -d "|" -f 1 file22
## OUTPUT

<img width="517" height="198" alt="Screenshot 2025-08-13 110944" src="https://github.com/user-attachments/assets/4caeeca7-875c-43b4-b373-4f2ebf13a9c3" />


cut -d "|" -f 2 file22
## OUTPUT
<img width="584" height="204" alt="Screenshot 2025-08-13 111018" src="https://github.com/user-attachments/assets/bea3fec6-c528-421e-8fdb-1f4b501bdf03" />


cat < newfile 
```
Hello world
hello world
^d
````
<img width="512" height="156" alt="Screenshot 2025-08-13 111058" src="https://github.com/user-attachments/assets/27af7d46-15a2-42f1-9f9f-a95b692a32cf" />


cat > newfile 
Hello world
hello world

<img width="516" height="163" alt="Screenshot 2025-08-13 111129" src="https://github.com/user-attachments/assets/ae349dfd-d699-46a0-966f-47c0b9f5cea9" />
 
grep Hello newfile 
## OUTPUT

<img width="510" height="118" alt="Screenshot 2025-08-13 111157" src="https://github.com/user-attachments/assets/e534c23f-2bb4-4352-a98e-cd8c6eab63a5" />


grep hello newfile 
## OUTPUT

<img width="513" height="123" alt="Screenshot 2025-08-13 111222" src="https://github.com/user-attachments/assets/87b3b347-ce04-43b7-a11f-568d9528937e" />



grep -v hello newfile 
## OUTPUT

<img width="519" height="117" alt="Screenshot 2025-08-13 111249" src="https://github.com/user-attachments/assets/750e1b9f-9c40-4856-ad3a-a2c4866ac88f" />


cat newfile | grep -i "hello"
## OUTPUT

<img width="644" height="156" alt="Screenshot 2025-08-13 111316" src="https://github.com/user-attachments/assets/70d2278b-2fc6-4b21-ae6d-ec1193c96bb6" />



cat newfile | grep -i -c "hello"
## OUTPUT

<img width="726" height="122" alt="Screenshot 2025-08-13 111349" src="https://github.com/user-attachments/assets/86bbcea3-4b79-4a8c-90fb-eb5c193fe7d3" />

grep -w -n world newfile   
## OUTPUT

<img width="590" height="163" alt="Screenshot 2025-08-13 111441" src="https://github.com/user-attachments/assets/dbde4aca-a6c8-4ebe-9f7d-a2939bef209f" />

cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```
<img width="566" height="291" alt="Screenshot 2025-08-13 111531" src="https://github.com/user-attachments/assets/b6d1e9a3-d1d1-4542-9716-9b9ea09e179d" />

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```

<img width="555" height="287" alt="Screenshot 2025-08-13 111553" src="https://github.com/user-attachments/assets/7c0663f4-dc9a-4333-aa94-e66a1620d17c" />

egrep -w 'Hello|hello' newfile 
## OUTPUT

<img width="667" height="153" alt="Screenshot 2025-08-13 111620" src="https://github.com/user-attachments/assets/1390e766-c0f2-489a-aba3-f495a95ba66d" />


egrep -w '(H|h)ello' newfile 
## OUTPUT

<img width="639" height="167" alt="Screenshot 2025-08-13 111649" src="https://github.com/user-attachments/assets/4afb13aa-ede0-4a68-be16-76cfb872285e" />


egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT

<img width="739" height="166" alt="Screenshot 2025-08-13 111724" src="https://github.com/user-attachments/assets/412f59b7-7374-4e7b-a3b0-beef330f77c0" />



egrep '(^hello)' newfile 
## OUTPUT

<img width="585" height="114" alt="Screenshot 2025-08-13 111748" src="https://github.com/user-attachments/assets/efaafaff-7ca4-4586-a1e4-00d4f2111e26" />


egrep '(world$)' newfile 
## OUTPUT

<img width="597" height="156" alt="Screenshot 2025-08-13 111813" src="https://github.com/user-attachments/assets/c6582b8e-f7b2-45a5-866a-6bcd2f1a4d28" />


egrep '(World$)' newfile 
## OUTPUT

<img width="573" height="125" alt="Screenshot 2025-08-13 111835" src="https://github.com/user-attachments/assets/1211521f-d729-4843-894d-66ca7e012ad6" />



egrep '((W|w)orld$)' newfile 
## OUTPUT

<img width="636" height="157" alt="Screenshot 2025-08-13 111905" src="https://github.com/user-attachments/assets/572d6ba5-3eb3-4874-b704-cb96ebd24bf6" />


egrep '[1-9]' newfile 
## OUTPUT

<img width="555" height="167" alt="Screenshot 2025-08-13 111959" src="https://github.com/user-attachments/assets/2336e3fa-5f4d-4a39-b500-d274c137516b" />


egrep 'Linux.*world' newfile 
## OUTPUT

<img width="659" height="122" alt="Screenshot 2025-08-13 112025" src="https://github.com/user-attachments/assets/399e949a-2df7-4c92-b40a-f1c722677e6b" />

egrep 'Linux.*World' newfile 
## OUTPUT

<img width="645" height="120" alt="Screenshot 2025-08-13 112047" src="https://github.com/user-attachments/assets/33e2841d-e5ca-4f82-ad61-f7a1ed433118" />


egrep l{2} newfile
## OUTPUT

<img width="517" height="164" alt="Screenshot 2025-08-13 112116" src="https://github.com/user-attachments/assets/c0f350f0-28fa-4293-9c6d-75da153b7647" />


egrep 's{1,2}' newfile
## OUTPUT 

<img width="564" height="204" alt="Screenshot 2025-08-13 112145" src="https://github.com/user-attachments/assets/c1cabb52-0ba8-41a7-ac85-80acb176bbfd" />

cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```

<img width="591" height="414" alt="Screenshot 2025-08-13 112221" src="https://github.com/user-attachments/assets/5b80ee12-2468-4cbe-87f2-6df00744e4fe" />


sed -n -e '3p' file23
## OUTPUT

<img width="518" height="122" alt="Screenshot 2025-08-13 112244" src="https://github.com/user-attachments/assets/b75d5ddd-429c-4f81-9bdb-965db40a0976" />


sed -n -e '$p' file23
## OUTPUT

<img width="512" height="109" alt="Screenshot 2025-08-13 112308" src="https://github.com/user-attachments/assets/6c235867-b2cb-433a-93a1-0e45ccf11d75" />


sed  -e 's/Ram/Sita/' file23
## OUTPUT

<img width="685" height="422" alt="Screenshot 2025-08-13 112331" src="https://github.com/user-attachments/assets/68d4fd4b-f038-4ae0-92d2-734b488598d3" />


sed  -e '2s/Ram/Sita/' file23
## OUTPUT

<img width="651" height="411" alt="Screenshot 2025-08-13 112353" src="https://github.com/user-attachments/assets/2cbb6be5-1b2e-4ffc-8c44-9056b22e94e9" />


sed  '/tom/s/5000/6000/' file23
## OUTPUT

<img width="690" height="414" alt="Screenshot 2025-08-13 112420" src="https://github.com/user-attachments/assets/7cdd087d-a49b-4946-b5a9-9062b35469d5" />


sed -n -e '1,5p' file23
## OUTPUT

<img width="622" height="290" alt="Screenshot 2025-08-13 112442" src="https://github.com/user-attachments/assets/7fb5d49d-a888-4818-86f9-c520ad4e35e4" />


sed -n -e '2,/Joe/p' file23
## OUTPUT

<img width="648" height="210" alt="Screenshot 2025-08-13 112508" src="https://github.com/user-attachments/assets/b20f826c-6fed-406a-887f-6b70802a0e48" />


sed -n -e '/tom/,/Joe/p' file23
## OUTPUT

<img width="686" height="160" alt="Screenshot 2025-08-13 112534" src="https://github.com/user-attachments/assets/214382e4-2cc6-45aa-92ab-4e7bfa2a7bc1" />


seq 10 
## OUTPUT

<img width="621" height="489" alt="Screenshot 2025-08-13 112603" src="https://github.com/user-attachments/assets/ef9f25b9-ef52-4340-9023-5ea24f528a70" />


seq 10 | sed -n '4,6p'
## OUTPUT

<img width="568" height="210" alt="Screenshot 2025-08-13 112621" src="https://github.com/user-attachments/assets/2f50d381-528d-4bc6-ae13-cf2eb2f7f631" />


seq 10 | sed -n '2,~4p'
## OUTPUT

<img width="537" height="201" alt="Screenshot 2025-08-13 112643" src="https://github.com/user-attachments/assets/01e208d3-f791-416c-a2f1-de1421cb4b25" />


seq 3 | sed '2a hello'
## OUTPUT

<img width="541" height="249" alt="Screenshot 2025-08-13 112702" src="https://github.com/user-attachments/assets/6fee50ab-79f7-42e0-8537-61c872c45787" />


seq 2 | sed '2i hello'
## OUTPUT

<img width="551" height="209" alt="Screenshot 2025-08-13 112725" src="https://github.com/user-attachments/assets/ebed5770-bb8d-42cb-97b1-383e9bf600c8" />

seq 10 | sed '2,9c hello'
## OUTPUT

<img width="603" height="204" alt="Screenshot 2025-08-13 112743" src="https://github.com/user-attachments/assets/c7c481cf-0e56-4425-9cd1-6b8b16777c33" />

sed -n '2,4{s/^/$/;p}' file23
## OUTPUT

<img width="663" height="216" alt="Screenshot 2025-08-13 112801" src="https://github.com/user-attachments/assets/cec4d4dc-67e7-491e-9bc7-c518f3ea450c" />


#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
## OUTPUT

<img width="978" height="281" alt="Screenshot 2025-08-13 112920" src="https://github.com/user-attachments/assets/1b5ed9ed-f6d1-4bb5-a374-4cdf69bbd9eb" />
<img width="598" height="295" alt="Screenshot 2025-08-13 112948" src="https://github.com/user-attachments/assets/2aafa8c6-6524-4aaf-873a-625be2e1b338" />

cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file22
uniq file22
## OUTPUT

<img width="598" height="331" alt="Screenshot 2025-08-13 113026" src="https://github.com/user-attachments/assets/2853ba52-5e60-4fcd-943c-635e6a115e8e" />

<img width="581" height="330" alt="Screenshot 2025-08-13 113047" src="https://github.com/user-attachments/assets/26e15710-843e-4301-8f28-01ed0862f235" />

<img width="583" height="284" alt="Screenshot 2025-08-13 113107" src="https://github.com/user-attachments/assets/73a29bc7-1450-43fc-b34a-b04f3154d2d3" />


#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
 
<img width="796" height="412" alt="Screenshot 2025-08-13 113128" src="https://github.com/user-attachments/assets/0b1b2d62-37e7-4230-989e-ecc0f5b6f7c6" />

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
<img width="511" height="204" alt="Screenshot 2025-08-13 113214" src="https://github.com/user-attachments/assets/341d41df-19dd-4cc4-91b1-ec4398e0c1d5" />

cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
<img width="511" height="209" alt="Screenshot 2025-08-13 113237" src="https://github.com/user-attachments/assets/d18df529-b0dc-4432-a98e-f5b52541866b" />

cat urllist.txt | tr -d ' '
 ## OUTPUT

<img width="607" height="201" alt="Screenshot 2025-08-13 113300" src="https://github.com/user-attachments/assets/907dc2c4-ec3d-44cc-9473-8e8fda706e5a" />

 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT

<img width="880" height="202" alt="Screenshot 2025-08-13 113327" src="https://github.com/user-attachments/assets/cbfae039-570c-40e1-936b-d5c2f1882844" />


#Backup commands
tar -cvf backup.tar *
## OUTPUT


mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 
tar -tvf backup.tar
## OUTPUT


tar -xvf backup.tar
## OUTPUT

gzip backup.tar

ls .gz
## OUTPUT
 
gunzip backup.tar.gz
## OUTPUT

 
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT


cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT

 
ls file1
## OUTPUT

echo $?
## OUTPUT 
./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 
abcd
 
echo $?
 ## OUTPUT


 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
##OUTPUT



chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT


# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT



# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT


# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 
 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 
 
cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 
 
 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
 
cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT
cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT


cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT

 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 
cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT



$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
 ./funcex.sh 

 
 ./funcex.sh 1 2

 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 


# RESULT:
The Commands are executed successfully.
