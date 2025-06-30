# DAY-3
I am Jaskiran kaur from department of 'COMPUTER SCIENCE ENGINEERING'.
Today, we will discuss about topi 'FILE AND DIRECTORY PERMISSION'. in this topic, we read commands, 
chmod: change mode
       this command is use for change mode.
       syntax; chmod +x filename.sh
       for run a file; ./filename.sh
       in this syntax, +x is a excuetable.
chmod 444: this commands is gives only permission.
         eg, $chmod 444 day3.sh
             $nano day3.sh
             in this syntax, fileday3.sh is unwriteable. 
chmod 644: this command gives only permission to owener for write something in file.
         eg, $ chmod 644 day3.sh
             $nano day3.sh

Command, ECHO: 
         this command is uses for print or create something. 
         use for write hello to file.
         .txt works for file.
         eg,  $ echo hello> day3.txt
              $ cat day3.txt       (for create & excess file.)
          hello 
          $ 

Use of Command ECHO:
The echo command is one of the most fundamental and frequently used commands in Linux and other Unix-like operating systems. Its primary purpose is to display a line of text or string to the standard output, which is typically your terminal.
1. Displaying Simple Text/Strings:
                           This is the most basic use.
                           Bash
                           echo "Hello, World!"
   
                           Output:
                           Hello, World!
2.  Displaying Variables:
                   echo is indispensable for viewing the values of environment variables or custom variables you've defined.
                   syntax: Bash
                   NAME="Alice"
                   echo "My name is $NAME"
                   echo "My current working directory is: $PWD"
                   echo "My default shell is: $SHELL"

                   Output (example):
                   My name is Alice
                   My current working directory is: /home/user
                   My default shell is: /bin/bash
3. Interpreting Escape Sequences (with -e option):
The -e option enables the interpretation of backslash escape sequences, allowing for special formatting or characters.

    \n: Newline
    \t: Horizontal tab
    \b: Backspace
    \r: Carriage return (moves cursor to the beginning of the line)
    \a: Alert (bell sound)
    \\: Backslash character
   \c: Suppresses the trailing newline and any text after it.

eg,  echo -e "Line 1\nLine 2"           # Prints on two separate lines
     echo -e "Name:\tJohn Doe"          # Prints with a tab
     echo -e "This is a test\b\b\bfile" # Backspaces, so output is "This is a file"
    echo -e "Counting: 10\rCounting: 20" # Overwrites "10" with "20"
    echo -e "Alert! \a"                # Plays a system sound
    echo -e "Part 1\cPart 2"           # Prints "Part 1" and no newline

4. Omitting the Trailing Newline (with -n option):
                          By default, echo adds a newline character at the end of its output. The -n option prevents this, which is useful for prompts or building output on                              the same line.
                                   syntax: Bash
                                           echo -n "Enter your name: "
                                           read NAME
                                           echo "Hello, $NAME!"

 5. Redirecting Output to a File:
                        echo is frequently used to write content to files.
                        >: Overwrites the file if it exists, creates it if it doesn't.
                        >>: Appends to the file if it exists, creates it if it doesn't.
Examples:
Bash
echo "This is some text for the file." > my_file.txt     # Create/overwrite
echo "This line will be appended." >> my_file.txt       # Append
echo "Username: $USER" >> /var/log/system_info.log      # Log information



