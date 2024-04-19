# AdjustTask
## Task 1: Play with File and Character
### Files Provided
- `file.txt`: Contains random strings provided in the challenge.
### 1. How many lines in this file?
To count the number of lines in the file, I used the following command:
```bash
wc -l file.txt
```
Result:
```
98 file.txt
 ```
### 2. How many “Z” Characters in this file ?
To count the number of “Z” Characters in the file, I used the following command:
```bash
grep -o 'Z' file.txt | wc -l
```
Result:
```
44
```
### 3. Find on which line is “Junior”, “Platform” and “Engineer”,not case sensitive.
To find on which line is “Junior”, “Platform” and “Engineer”,not case sensitive in the file, I used the following commands:
```bash
grep -in 'Junior' file.txt
```
```bash
grep -in 'Platform' file.txt
```
```bash
grep -in 'Engineer' file.txt
```
Results:
```
65:x7t2vMJunior0qcMHQtnVGhlggfnry
 ```
```
28:COJILxEOhBRPlatFormjc00OhTT6ve
 ```
```
88:7B6nmS3lLJaEngineeR28pzseTejdm
 ```
### 4. Change “Junior” to “Senior”
To change “Junior” to “Senior” in the file, I used the following command:
```bash
 sed -i 's/Junior/Senior/gI' file.txt
```
Result:
In order to verify the result, I used the following command ``grep -in 'senior' file.txt``  and I obtained the following result:``65:x7t2vMSenior0qcMHQtnVGhlggfnry
``



