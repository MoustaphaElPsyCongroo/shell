# Shell - loops, conditions and parsing

## Learning Objectives

### General

* How to create SSH keys
* What is the advantage of using  `#!/usr/bin/env bash` over `#!/bin/bash`
* How to use `while`, `until` and `for` loops
* How to use `if`, `else`, `elif` and `case` condition statements
* How to use the `cut` command
* What are files and other comparison operators, and how to use them



## Scripts and exercices descriptions
### 0-RSA_public_key.pub
Create a RSA key pair, share the public key here

### 1-for_best_school
Write a Bash script that displays `Best School` 10 times.

Requirement:

* You must use the `for` loop (`while` and `until` are forbidden)

### 2-while_best_school
Write a Bash script that displays `Best School` 10 times.

Requirements:

* You must use the `while` loop (`for` and `until` are forbidden)

### 3-until_best_school
Write a Bash script that displays `Best School` 10 times.

Requirements:

* You must use the `until` loop (`for` and `while` are forbidden)

### 4-if_9_say_hi
Write a Bash script that displays `Best School` 10 times, but for the 9th iteration, displays `Best School` _and then_ `Hi` on a new line.

Requirements:

* You must use the `while` loop (`for` and `until` are forbidden)
* You must use the `if` statement

### 5-4_bad_luck_8_is_your_chance
Write a Bash script that loops from 1 to 10 and:

* displays `bad luck` for the 4th loop iteration
* displays `good luck` for the 8th loop iteration
* displays `Best School` for the other iterations

Requirements:

* You must use the `while` loop (`for` and `until` are forbidden)
* You must use the `if`, `elif` and `else` statements

### 6-superstitious_numbers
Write a Bash script that displays numbers from 1 to 20 and:

* displays `4` _and then_ `bad luck from China` for the 4th loop iteration
* displays `9` _and then_ `bad luck from Japan` for the 9th loop iteration
* displays `17` _and then_ `bad luck from Italy` for the 17th loop iteration

Requirements:

* You must use the `while` loop (`for` and `until` are forbidden)
* You must use the `case` statement

### 7-clock
Write a Bash script that displays the time for 12 hours and 59 minutes:

* display hours from 0 to 12
* display minutes from 1 to 59

Requirements:

* You must use the `while` loop (`for` and `until` are forbidden)

### 8-for_ls
Write a Bash script that displays:

* The content of the current directory
* In a list format
* Where only the part of the name after the first dash is displayed (refer to the example)

Requirements:

* You must use the `for` loop (`while` and `until` are forbidden)
* Do not display hidden files

### 9-to_file_or_not_to_file
Write a Bash script that gives you information about the `school` file.

Requirements:

* You must use `if` and, `else` (`case` is forbidden)
* Your Bash script should check if the file exists and print:

    * if the file exists: `school file exists`
    * if the file does not exist: `school file does not exist`

* If the file exists, print:

    * if the file is empty: `school file is empty`
    * if the file is not empty: `school file is not empty`
    * if the file is a regular file: `school is a regular file`
    * if the file is not a regular file: (nothing)

### 10-fizzbuzz
Write a Bash script that displays numbers from 1 to 100.

Requirements:

* Displays `FizzBuzz` when the number is a multiple of 3 and 5
* Displays `Fizz` when the number is multiple of 3
* Displays `Buzz` when the number is a multiple of 5
* Otherwise, displays the number
* In a list format

### 11-read_and_cut
Write a Bash script that displays the content of the file `/etc/passwd`.

Your script should only display:

* username
* user id
* Home directory path for the user

Requirements:

* You must use the `while` loop (`for` and `until` are forbidden)

### Write a Bash script that displays the content of the file `/etc/passwd`, using the `while` loop + IFS.

Format: `The user USERNAME is part of the GROUP_ID gang, lives in HOME_DIRECTORY and rides COMMAND/SHELL. USER ID's place is protected by the passcode PASSWORD, more info about the user here: USER ID INFO`

Requirements:

* You must use the `while` loop (`for` and `until` are forbidden)

### 13-lets_parse_apache_logs
Write a Bash script that displays the visitor IP along with the HTTP satus code from the Apache log file.

Requirement:

* Format: IP HTTP_CODE

    * in a list format
    * See example

* You must use `awk`
* You are not allowed to use `while`, `for`, `until` and `cut`

### 14-dig_the-data
Using what you did in the previous exercise, write a Bash script that groups visitors by IP and HTTP status code, and displays this data.

Requirements:

* The exact format must be:

    * OCCURENCE_NUMBER IP HTTP_CODE
    * In list format

* Ordered from the greatest to the lowest number of occurrences

    * See example

* You must use `awk`
* You are not allowed to use `while`, `for`, `until` and `cut`
