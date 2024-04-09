# Internet & Linux Programming

## 0. Prologue

* Zhang Jian
  * jianzh@bjtu.edu.cn
  * Please include "[Linux 2024]" in your email topic
* Evaluation Criteria
  * 60pt, 6 Assignments
  * 10pt, 2~3 Quiz
  * 30pt, Final Report
  * up to 5pt, Performance Bonus

## 1. Introduction

* Story

* Philosophy & Priciples

> The linux philosophy is "Laugh in face of danger". Oops. Wrong one. "Do it yourself". That's it.
>
> Linus Tarvolds

## 2. Shell Basics

* Getting Started
  * file, process, directory, symbolic link
* Shell
* Shell Usage
* Variables

* Takeaways
  * Using **rm** carefully
  * Environment Variables;

* Commands
  * etc..
  * Output redirection
    * `cat a.txt > b.txt`: overwrite
    * `cat a.txt >> b.txt`: append
  * Error redirection
    * `./bin 2> log.txt`
  * Input redirection
    * 
  * Merge 2 streams
    * `command 2>&1 | ...`: merge stdout and stderr
  * Split to 2 streams
    * `command | tee file1 file2`

* File Structure  

* File Authority & Links

* Job control
  * `ps aux`, `htop`, etc..
  * `ctrl + c`: interrupt
  * `ctrl + d`: EOF
  * `ctrl + z`: suspend
  * use `&` in the end of command: run in background
  * `nohup ... > log &`: suspend a process to background

* Pipe



