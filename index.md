## `find` Commmand Line Options
source links: [Link](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/) [Link](https://www.redhat.com/sysadmin/linux-find-command)
* `-empty`: this option is to search for all empty files or directories in the entered directory. For example the following input will search for empty files or directories. (the current directory is ~/Desktop/cse15L)
* input: `$ find -empty`
* output: the command should return the empty folder I created in this current directory, `./Empty_Directory`
* input: `$ find -empty` this time I created an empty file in the current directory named `Empty_File`
* output: the command should return the empty folder and the new empty file I created
```
./Empty Directory
./Empty_File.txt
```
* `-name`: this option finds things with a specific name (the current directory is ~/Desktop/cse15L).
* input: `$ find -name cse15l-lab-reports.pdf`
* output: `./cse15l-lab-reports.pdf`
* input: `$ find -name *.txt` this will find all txt files in the current directory
* output: this should only return the file I created above as that file is the only txt file in the current directory. `./Empty_File.txt`
* `-type`: this option finds things by the type of that file or directory (the current directory is ~/Desktop/cse15L)
* input: `$ find -type d" *`
* output: the command shows all directories in the current directory
```
.
./Empty Directory
```
* input: `$ find -type f`
* output: the command shows all the files in current directory
```
./Bugs1.jpg
./cdCommand1.JPG
./cdCommand2.JPG
./cse15l-lab-reports.pdf
./Empty_File.txt
./grep Commmand Line Options _ Lab-Report-3.pdf
./Handler.class
./Lab-report-4.pdf
./lsCommand.JPG
./OptionEmpty.JPG
./passWordReset1.JPG
./passWordReset2.JPG
./pwdCommand.JPG
./remoteConnecting.JPG
./Server.class
./Server.java
./ServerHttpHandler.class
./StringServer _ cse15L-Lab-Report2.pdf
./StringServer.class
./StringServer.java
./StringServer1.JPG
./StringServer2.JPG
./StringServer3.JPG
./test.java
./URLHandler.class
./VScode.JPG
```
* `-ls` : this option command shows everything in the entered location or current directory  
* input: `$ find -ls"`(current directory is ~/Desktop/cse15L)
* output:
```
36310271995696278      8 drwxr-xr-x   1 Shan     197609          0 Mar 13 20:48 .
10696049115191633     32 -rw-r--r--   1 Shan     197609      32325 Jan 30 21:46 ./Bugs1.jpg
18858823439741209     16 -rw-r--r--   1 Shan     197609      14328 Jan 16 19:26 ./cdCommand1.JPG
48413695994278116     20 -rw-r--r--   1 Shan     197609      17855 Jan 16 19:27 ./cdCommand2.JPG
16325548649391667    420 -rw-r--r--   1 Shan     197609     427379 Jan 29 00:54 ./cse15l-lab-reports.pdf
48976645947743546      0 drwxr-xr-x   1 Shan     197609          0 Mar 13 20:35 ./Empty\ Directory
 7881299347963979      0 -rw-r--r--   1 Shan     197609          0 Mar 13 20:48 ./Empty_File.txt
21673573206763088    100 -rw-r--r--   1 Shan     197609     101519 Feb 13 20:46 ./grep\ Commmand\ Line\ Options\ _\ Lab-Report-3.pdf
19984723346659668      4 -rw-r--r--   1 Shan     197609       1249 Jan 30 20:14 ./Handler.class
14636698789039348   1500 -rw-r--r--   1 Shan     197609    1532399 Feb 27 23:37 ./Lab-report-4.pdf
34339947158846435     84 -rw-r--r--   1 Shan     197609      81969 Jan 16 19:22 ./lsCommand.JPG
13510798882288779     16 -rw-r--r--   1 Shan     197609      15724 Mar 13 20:44 ./OptionEmpty.JPG
15762598695990817     52 -rw-r--r--   1 Shan     197609      52562 Jan 28 22:53 ./passWordReset1.JPG
32932572275378313     28 -rw-r--r--   1 Shan     197609      24721 Jan 29 00:13 ./passWordReset2.JPG
13510798882283723     12 -rw-r--r--   1 Shan     197609      11883 Jan 16 19:26 ./pwdCommand.JPG
41376821576513900     36 -rw-r--r--   1 Shan     197609      33282 Jan 16 19:12 ./remoteConnecting.JPG
 9851624185076069      4 -rw-r--r--   1 Shan     197609       1335 Jan 30 20:14 ./Server.class
 7881299348092161      4 -rw-r--r--   1 Shan     197609       1871 Jan 30 20:09 ./Server.java
22799473113766244      4 -rw-r--r--   1 Shan     197609       1072 Jan 30 20:14 ./ServerHttpHandler.class
45035996273899003    276 -rw-r--r--   1 Shan     197609     279676 Jan 30 23:26 ./StringServer\ _\ cse15L-Lab-Report2.pdf
 8162774324812131      4 -rw-r--r--   1 Shan     197609        723 Jan 30 20:14 ./StringServer.class
13510798882298306      4 -rw-r--r--   1 Shan     197609        865 Feb  1 19:35 ./StringServer.java
13229323905594813     20 -rw-r--r--   1 Shan     197609      18659 Jan 30 20:27 ./StringServer1.JPG
33495522228767137     20 -rw-r--r--   1 Shan     197609      18954 Jan 30 20:47 ./StringServer2.JPG
20266198323360862     20 -rw-r--r--   1 Shan     197609      19735 Jan 30 21:08 ./StringServer3.JPG
191965934116677440      1 -rw-r--r--   1 Shan     197609        515 Jan 18 15:54 ./test.java
 19703248369949018      1 -rw-r--r--   1 Shan     197609        158 Jan 30 20:14 ./URLHandler.class
 32369622321765964     72 -rw-r--r--   1 Shan     197609      73441 Jan 16 18:46 ./VScode.JPG
```
* input: `$ find ~/Desktop/cse12 -ls`
* output: 
```
37999121856017107      8 drwxr-xr-x   1 Shan     197609          0 Mar  8 18:43 /c/Users/Henry/Desktop/cse12
 8444249301386283      0 drwxr-xr-x   1 Shan     197609          0 Jan 11 18:54 /c/Users/Henry/Desktop/cse12/.vscode
 3659174697970862      1 -rw-r--r--   1 Shan     197609        199 Jan 11 18:54 /c/Users/Henry/Desktop/cse12/.vscode/settings.json
19421773393153681      4 drwxr-xr-x   1 Shan     197609          0 Jan 26 02:43 /c/Users/Henry/Desktop/cse12/cse12-wi23-pa1-RPS-starter-main
 7881299348104028      0 drwxr-xr-x   1 Shan     197609          0 Jan 26 02:43 /c/Users/Henry/Desktop/cse12/cse12-wi23-pa1-RPS-starter-main/.vscode
 6192449487840099      1 -rw-r--r--   1 Shan     197609        221 Jan 26 02:43 /c/Users/Henry/Desktop/cse12/cse12-wi23-pa1-RPS-starter-main/.vscode/settings.json
 7881299348019765      0 drwxr-xr-x   1 Shan     197609          0 Jan 11 19:50 /c/Users/Henry/Desktop/cse12/cse12-wi23-pa1-RPS-starter-main/libs
...(changed to ... for privacy)
  9007199254969921      4 -rw-r--r--   1 Shan     197609       3622 Feb 23 06:07 /c/Users/Henry/Desktop/cse12/submit/CustomTester.java
  9851624185101891      4 -rw-r--r--   1 Shan     197609       3949 Feb 23 06:07 /c/Users/Henry/Desktop/cse12/submit/Sanctuary.java
  8444249301548614      4 -rw-r--r--   1 Shan     197609       2409 Feb 23 06:08 /c/Users/Henry/Desktop/cse12/submit/Student.java
 62205969853197092      8 -r--r--r--   1 Shan     197609       4226 Feb 23 06:11 /c/Users/Henry/Desktop/cse12/submit.zip
```
