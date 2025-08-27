### NAME : HARSHAT . G
### REG NO.: 212224040106
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
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files
cat < file1
cat < file2
# Comparing Files
cmp file1 file2
## OUTPUT
<img width="421" height="312" alt="os1" src="https://github.com/user-attachments/assets/a862f3a9-a817-40cb-8952-35f6e6776d4f" />
comm file1 file2
## OUTPUT
<img width="463" height="767" alt="Screenshot 2025-08-27 164007" src="https://github.com/user-attachments/assets/af4971fe-cafb-4bc2-bbd1-eca0b344946c" />
diff file1 file2
## OUTPUT
<img width="442" height="253" alt="image" src="https://github.com/user-attachments/assets/5bc4909c-d79a-43d2-8ba3-abff9d8a8967" />
### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
cut -c1-3 file11
## OUTPUT
<img width="455" height="88" alt="image" src="https://github.com/user-attachments/assets/81ea8d54-1d0e-416f-958d-384717617305" />
cut -d "|" -f 1 file22
## OUTPUT
<img width="455" height="88" alt="image" src="https://github.com/user-attachments/assets/642d8f09-03c0-4a13-a9e5-c7c482610c2a" />
cut -d "|" -f 2 file22
## OUTPUT
<img width="455" height="88" alt="image" src="https://github.com/user-attachments/assets/cc19da93-50ae-411a-aee0-5c09b5186f16" />
cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 
Hello world
hello world
 
grep Hello newfile 
## OUTPUT
<img width="455" height="50" alt="image" src="https://github.com/user-attachments/assets/f8e3e4e4-2c18-48f1-b6cb-f210e3084cf3" />
grep hello newfile 
## OUTPUT
<img width="521" height="65" alt="image" src="https://github.com/user-attachments/assets/de195b27-6aa7-4f56-8b4e-45f2d855a6fc" />
grep -v hello newfile 
## OUTPUT
<img width="532" height="46" alt="image" src="https://github.com/user-attachments/assets/a12d180c-e3b2-4127-9265-91f2b14d6ed1" />
cat newfile | grep -i "hello"
## OUTPUT
<img width="532" height="66" alt="image" src="https://github.com/user-attachments/assets/2ced3d10-5edf-443b-a581-c859160c3b29" />
cat newfile | grep -i -c "hello"
## OUTPUT
<img width="559" height="48" alt="image" src="https://github.com/user-attachments/assets/2e85506a-9fba-4ffa-a7e9-57770ccf3cd1" />
grep -R ubuntu /etc
## OUTPUT
<img width="1443" height="921" alt="image" src="https://github.com/user-attachments/assets/05dc76cc-daca-4219-bce5-3101ef95b9e0" />
grep -w -n world newfile   
## OUTPUT
<img width="568" height="66" alt="image" src="https://github.com/user-attachments/assets/4012e605-e69e-4ade-86b1-e7286e4f9989" />
cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
egrep -w 'Hello|hello' newfile 
## OUTPUT
<img width="568" height="66" alt="image" src="https://github.com/user-attachments/assets/45c27a06-2b92-40d7-b512-0f81941147da" />
egrep -w '(H|h)ello' newfile 
## OUTPUT
<img width="568" height="66" alt="image" src="https://github.com/user-attachments/assets/86779186-05b8-47e3-a51b-f7ed10a9e2ac" />
egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
<img width="568" height="66" alt="image" src="https://github.com/user-attachments/assets/a4a1967e-27a9-4416-9242-f5339b7025d1" />
egrep '(^hello)' newfile 
## OUTPUT
<img width="570" height="45" alt="image" src="https://github.com/user-attachments/assets/5e5a45b1-c65b-4aeb-8049-655b919c2d73" />
egrep '(world$)' newfile 
## OUTPUT
<img width="580" height="82" alt="image" src="https://github.com/user-attachments/assets/fbe04c49-f609-420a-ad1d-6886c74815a7" />
egrep '(World$)' newfile 
## OUTPUT
<img width="580" height="82" alt="image" src="https://github.com/user-attachments/assets/d31ab17d-b429-43d6-87a3-dbdcf66ddedb" />
egrep '((W|w)orld$)' newfile 
## OUTPUT
<img width="580" height="106" alt="image" src="https://github.com/user-attachments/assets/422adbb9-6a2c-4398-afd5-550e94b05154" />
egrep '[1-9]' newfile 
## OUTPUT
<img width="587" height="75" alt="image" src="https://github.com/user-attachments/assets/5adf730e-3d60-464b-b986-4c7494bb238f" />
egrep 'Linux.*world' newfile 
## OUTPUT
<img width="587" height="75" alt="image" src="https://github.com/user-attachments/assets/b0cb09a2-9ef6-4bd4-b492-689e7bbd8ac4" />
egrep 'Linux.*World' newfile 
## OUTPUT
<img width="587" height="75" alt="image" src="https://github.com/user-attachments/assets/9519a15e-6a73-436f-bdf5-1e3ce6c7e523" />
egrep l{2} newfile
## OUTPUT
<img width="587" height="75" alt="image" src="https://github.com/user-attachments/assets/3e4477db-e91f-4896-9dea-450daf942533" />
egrep 's{1,2}' newfile
## OUTPUT 
<img width="587" height="75" alt="image" src="https://github.com/user-attachments/assets/7cb19ef7-0393-4957-808c-f6dcc2cf0f66" />
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


sed -n -e '3p' file23
## OUTPUT
<img width="575" height="254" alt="image" src="https://github.com/user-attachments/assets/0b78a5b5-e65b-4273-a762-7c4646ef5db1" />
sed -n -e '$p' file23
## OUTPUT
<img width="575" height="113" alt="image" src="https://github.com/user-attachments/assets/8c3c9389-afe2-408e-a183-e3287e7fb7fc" />
sed  -e 's/Ram/Sita/' file23
## OUTPUT
<img width="625" height="199" alt="image" src="https://github.com/user-attachments/assets/2d4caf09-3c7a-45d8-b0cb-71273929f03b" />
sed  -e '2s/Ram/Sita/' file23
## OUTPUT
<img width="625" height="199" alt="image" src="https://github.com/user-attachments/assets/8627e139-f23c-4fa5-a87b-3e92c6033bbf" />
sed  '/tom/s/5000/6000/' file23
## OUTPUT
<img width="625" height="199" alt="image" src="https://github.com/user-attachments/assets/cc4ab7d3-6cb6-4714-a8c4-2ff508abb91e" />
sed -n -e '1,5p' file23
## OUTPUT
<img width="635" height="146" alt="image" src="https://github.com/user-attachments/assets/f88f767a-d806-4606-ad04-8dabc5aa97ac" />
sed -n -e '2,/Joe/p' file23
## OUTPUT
<img width="645" height="89" alt="image" src="https://github.com/user-attachments/assets/924c2620-07ec-46a3-ab03-c1030fc106ce" />
seq 10 
## OUTPUT
<img width="638" height="231" alt="image" src="https://github.com/user-attachments/assets/d5fd21ca-7ad0-44c9-a40b-22fbfc39ca38" />
seq 10 | sed -n '4,6p'
## OUTPUT
<img width="647" height="110" alt="image" src="https://github.com/user-attachments/assets/4fb9c809-cd12-4746-957a-e6f0ca8e56b7" />
seq 10 | sed -n '2,~4p'
## OUTPUT
<img width="647" height="110" alt="image" src="https://github.com/user-attachments/assets/e3cbd532-031e-4ff6-96d1-eab296946c33" />
seq 3 | sed '2a hello'
## OUTPUT
<img width="647" height="126" alt="image" src="https://github.com/user-attachments/assets/41812056-190b-4620-9091-20e802761661" />
seq 2 | sed '2i hello'
## OUTPUT
<img width="652" height="105" alt="image" src="https://github.com/user-attachments/assets/e1244b98-6550-4f7b-8a64-ad084a45d27f" />
seq 10 | sed '2,9c hello'
## OUTPUT
<img width="652" height="105" alt="image" src="https://github.com/user-attachments/assets/b4cfd6ee-d32e-4891-9341-5df05fbdc015" />
sed -n '2,4{s/^/$/;p}' file23
## OUTPUT
<img width="652" height="105" alt="image" src="https://github.com/user-attachments/assets/9771eafb-ea51-4942-8289-3d10e09c8278" />
sed -n '2,4{s/$/*/;p}' file23


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
<img width="676" height="249" alt="image" src="https://github.com/user-attachments/assets/da0baa93-e901-4f6b-90c9-c6fe5a353b7d" />
cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT
<img width="599" height="268" alt="image" src="https://github.com/user-attachments/assets/5854b33b-edd4-4cce-9f2a-24cd97757b63" />
cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
## OUTPUT
<img width="616" height="197" alt="image" src="https://github.com/user-attachments/assets/24fd7258-2d84-44ec-86b9-66a14201d544" />
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT
<img width="656" height="110" alt="image" src="https://github.com/user-attachments/assets/8cffb50f-0d31-4716-8979-b0838fbe00a5" />
#Backup commands
tar -cvf backup.tar *
## OUTPUT
<img width="1129" height="946" alt="image" src="https://github.com/user-attachments/assets/8b299f85-05fd-41ba-82c3-57ec48cf3d35" />
mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 
tar -tvf backup.tar
## OUTPUT
<img width="1456" height="994" alt="image" src="https://github.com/user-attachments/assets/bbc9d3f8-25d0-4c31-ad35-ef6169287319" />
tar -xvf backup.tar
## OUTPUT
<img width="910" height="1012" alt="image" src="https://github.com/user-attachments/assets/6eda518e-3afd-490f-a69a-a6cb0e413a71" />
gzip backup.tar
ls .gz
## OUTPUT
<img width="910" height="75" alt="image" src="https://github.com/user-attachments/assets/b1ea59e1-3b71-4bf4-a515-2f669483c9e5" />
gunzip backup.tar.gz
## OUTPUT
<img width="910" height="109" alt="image" src="https://github.com/user-attachments/assets/77242aa3-6fc7-4b70-afa7-284999600cd4" />
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT
<img width="910" height="219" alt="image" src="https://github.com/user-attachments/assets/b1c044ed-a7d0-4daa-9ece-69e16763da43" />
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT
<img width="913" height="200" alt="image" src="https://github.com/user-attachments/assets/1faa1d9c-864d-4919-824e-b78af5df86d0" />
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
<img width="915" height="772" alt="image" src="https://github.com/user-attachments/assets/62b7e2fb-8bd4-4ea0-bdf5-50232b97434b" />
ls file1
## OUTPUT
<img width="915" height="772" alt="image" src="https://github.com/user-attachments/assets/4416ea06-92bf-4d6e-8605-935cc8f78055" />
echo $?
## OUTPUT 
<img width="883" height="74" alt="image" src="https://github.com/user-attachments/assets/da4d8096-8289-4302-b29a-9cb38b4bb598" />
./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT
<img width="883" height="74" alt="image" src="https://github.com/user-attachments/assets/8faa78c7-fe1f-4f1e-839e-517a2d6c3a7e" />
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
## OUTPUT
<img width="885" height="394" alt="image" src="https://github.com/user-attachments/assets/540d235d-e933-442b-9e58-c7b828e96c4c" />
chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT
<img width="882" height="125" alt="image" src="https://github.com/user-attachments/assets/42194a21-3b49-4e47-9752-0a2579283cb9" />
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
<img width="893" height="320" alt="image" src="https://github.com/user-attachments/assets/3766441a-e21b-4af9-9b80-1f39fe0b3d4b" />
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
<img width="855" height="719" alt="image" src="https://github.com/user-attachments/assets/c8136f2b-5cab-412c-bc81-a023561c9c10" />
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
## OUTPUT
<img width="814" height="378" alt="image" src="https://github.com/user-attachments/assets/f98451fe-7b75-4f53-adf0-9881a63675b7" />
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
## OUTPUT
<img width="822" height="467" alt="image" src="https://github.com/user-attachments/assets/39834895-8d71-47b7-b7f5-e94031dc69e6" />
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
<img width="825" height="450" alt="image" src="https://github.com/user-attachments/assets/432da3b1-c232-4253-b611-242e78ab218f" />
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
<img width="830" height="250" alt="image" src="https://github.com/user-attachments/assets/9424291e-8c3e-4531-8b13-c9bff018945e" />
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
<img width="851" height="302" alt="image" src="https://github.com/user-attachments/assets/7cef187c-c044-4cb0-aee0-0fe6189b8268" />

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
<img width="895" height="411" alt="image" src="https://github.com/user-attachments/assets/83906523-eb5d-41ed-b1ec-0cf838e75be5" />
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
<img width="637" height="307" alt="image" src="https://github.com/user-attachments/assets/259a929b-a6da-445c-93a7-32e9e6d2a7d9" />
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
<img width="669" height="342" alt="image" src="https://github.com/user-attachments/assets/ceb2e3bc-6474-402e-9290-4195618b507a" />
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
<img width="700" height="311" alt="image" src="https://github.com/user-attachments/assets/a76561e0-4000-4bec-8cf1-d237c74fe7e2" />
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
<img width="716" height="336" alt="image" src="https://github.com/user-attachments/assets/0717a93f-869f-4be6-869a-78cb942b2ff5" />
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
<img width="727" height="286" alt="image" src="https://github.com/user-attachments/assets/0cdab4b6-ecb0-4e73-9d45-dc7b903d4aa3" />
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
<img width="717" height="286" alt="image" src="https://github.com/user-attachments/assets/ce20c563-8194-4f21-b55a-6d6294aec5da" />
cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT
<img width="768" height="503" alt="image" src="https://github.com/user-attachments/assets/a639012d-0740-4437-9300-97856c4cec00" />
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
<img width="731" height="362" alt="image" src="https://github.com/user-attachments/assets/bc1e36e6-efbd-4d5b-9b3e-ad7faeb2aa4f" />
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
<img width="658" height="386" alt="image" src="https://github.com/user-attachments/assets/4511fa94-e8dc-440e-8cb9-e1bcb7aa740b" />
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
<img width="440" height="226" alt="image" src="https://github.com/user-attachments/assets/893bf0e5-9466-4f1a-9cf1-d1a295a2208e" />
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
<img width="440" height="226" alt="image" src="https://github.com/user-attachments/assets/ab9e2349-cf64-4a36-8b7b-749e6740eca3" />
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
<img width="513" height="323" alt="image" src="https://github.com/user-attachments/assets/54fd9ef6-fff1-4a96-8b0e-309466ee61d2" />
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
<img width="581" height="541" alt="image" src="https://github.com/user-attachments/assets/6133cf90-9895-44f2-a71b-7db244f65056" />
# RESULT:
The Commands are executed successfully.
