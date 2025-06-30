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

3.  Displaying Variables:
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

4. Interpreting Escape Sequences (with -e option):
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

5. Omitting the Trailing Newline (with -n option):
                          By default, echo adds a newline character at the end of its output. The -n option prevents this, which                             is useful for prompts or building output on the same line.

                                           syntax: Bash
                                           echo -n "Enter your name: "
                                           read NAME
                                           echo "Hello, $NAME!"

 6. Redirecting Output to a File:
                        echo is frequently used to write content to files.
                        >: Overwrites the file if it exists, creates it if it doesn't.
                        >>: Appends to the file if it exists, creates it if it doesn't.

                        Examples:
                                Bash
                                echo "This is some text for the file." > my_file.txt     # Create/overwrite
                                echo "This line will be appended." >> my_file.txt       # Append
                                echo "Username: $USER" >> /var/log/system_info.log      # Log information


# What is a Pipe?

At its core, a pipe is a one-way communication channel that connects the standard output (stdout) of one command to the standard input (stdin) of another command. It essentially acts as a temporary buffer in memory.


# SHELL PROGRAMING EXAMPLES: 
)

example no. 1, 
        print variables

![WhatsApp Image 2025-06-30 at 10 29 22 AM](https://github.com/user-attachments/assets/5357aa8a-7a9f-401f-9354-9f3d20eb759b)

![WhatsApp Image 2025-06-30 at 10 29 34 AM](https://github.com/user-attachments/assets/9d0098c9-60a6-40bc-babd-880874ed3cf8)


![WhatsApp Image 2025-06-30 at 10 29 48 AM](https://github.com/user-attachments/assets/418520c6-b527-4e28-815b-2d2840fd3706)

       
![WhatsApp Image 2025-06-30 at 10 30 02 AM](https://github.com/user-attachments/assets/be5032ec-e1a8-4eda-ba9d-489bbd4cb58f)



example no. 2 
      print multiplication.

  ![WhatsApp Image 2025-06-30 at 11 00 52 AM](https://github.com/user-attachments/assets/24748abc-4619-45fb-95dd-3a97e5c7eaef)

  ![WhatsApp Image 2025-06-30 at 11 01 03 AM](https://github.com/user-attachments/assets/d43946c6-92d0-4ee9-923a-0358edc64860)



Then (DAY4) we learn about topic FILE COMPRESSION:
File compression is the process of reducing the size of a digital file while retaining all (or most) of its original information. The primary goals of file compression are:
  Saving Storage Space
  Faster Data Transmission
  Efficient Archiving 

  in this topic we learn about GZIP command:
                       syntax, filename.gz
                      eg, gzip notes.txt (for creates notes.txt.gz)
                          and delete (notes.txt)

![WhatsApp Image 2025-06-30 at 11 25 13 AM](https://github.com/user-attachments/assets/aaa6ac3d-82c4-4b17-b81b-c8af2dc581b6)


# WILDCARDS:
Wildcards in Linux are special characters used in the shell (like Bash) to create patterns that match multiple file or directory names. They are an essential tool for working efficiently on the command line, allowing you to select and operate on groups of files with a single command.

Here are the most common wildcards:

   1. * (Asterisk): Matches zero or more characters.
                   Example: ls *.txt will list all files ending with .txt 

 2. ? (Question Mark): Matches exactly one single character.
                 Example: ls photo?.jpg will list photo1.jpg, photoA.jpg, but not photo10.jpg (as 10 is two characters).
    
3. [] (Square Brackets): Matches a single character from a specified set or range.
                 Example (Set): ls report_[135].txt will list report_1.txt, report_3.txt, report_5.txt

   here is the table of wildcards:
   ![WhatsApp Image 2025-06-30 at 11 31 57 AM](https://github.com/user-attachments/assets/1299622b-7a1e-4130-8aff-b37757c9d84f)

# ESCAPE CHARACTERS:
 Escape characters are special symbols used in programming, command-line interfaces, and various text formats to change the literal meaning of the character(s) that immediately follow them. Their primary purpose is to allow you to:
       Represent special characters
       Suppress special meaning

here are some escaping characters:
 1. \n (Newline): Moves the cursor to the beginning of the next line.
Bash

echo -e "Hello\nWorld"
# Output:
# Hello
# World

 2. \t (Horizontal Tab): Inserts a tab space.
Bash

echo -e "Name:\tJohn Doe"
# Output:
# Name:   John Doe

 3. \r (Carriage Return): Moves the cursor to the beginning of the current line, overwriting previous text.
Bash

echo -e "Progress: 10%\rProgress: 100%"
# Output:
# Progress: 100%

 4. \b (Backspace): Moves the cursor back one character, potentially overwriting.
Bash

echo -e "abc\b\bdef" # Deletes 'c' and 'b', then prints 'def'
# Output:
# adef

 5. \a (Alert/Bell): Produces an audible bell sound (if your terminal supports it).
Bash

echo -e "System alert! \a"

 6. \\ (Literal Backslash): To print a backslash itself, you need to escape it.
Bash

echo -e "Path: C:\\Users\\Name"
# Output:
# Path: C:\Users\Name


Scenario 2: Escaping Shell Metacharacters (Suppressing Special Meaning)

The shell (Bash, Zsh, etc.) assigns special meanings to various characters (called metacharacters). If you want to use these characters literally within a command or string, you must escape them.

1.  Spaces and Tabs:
    If a filename or directory name contains spaces, you must quote it or escape the spaces to prevent the shell from                 interpreting the words as separate arguments.
    Bash

# Incorrect: shell sees "my" and "document.txt" as two separate arguments
# touch my document.txt

# Correct way to create a file with spaces:
touch "my document.txt" # Using double quotes
touch my\ document.txt  # Using backslash to escape the space

 2. Wildcards (*, ?, []):
    If you have a file named my*file.txt and you want to refer to that specific file (not files matching the my*.txt pattern),        you escape the asterisk.
    Bash

   touch 'my*file.txt' # Create the file first

   ls my\*file.txt    # Escaping the asterisk
   ls 'my*file.txt'   # Quoting the entire string (easier for multiple special chars)
   ls "my*file.txt"   # Double quotes also work, but allow variable expansion

 3. Command Separators (&, ;, |):
    If you want to use these characters as part of a string rather than as command operators.
    Bash

    echo "This is a test \& more" # & is a background operator normally
    # Output:
    # This is a test & more

    echo "Part 1\;Part 2" # ; separates commands normally
    # Output:
    # Part 1;Part 2

 4. Quotes (', "):
    To include a quote character within a string that is already delimited by the same type of quotes.
    Bash

    echo 'She said, "Hello!"' # Inner double quotes are fine within single quotes
    echo "He said, \"Hi!\""  # Escaping inner double quote within double quotes
    # Output:
    # She said, "Hello!"
    # He said, "Hi!"

 5. **Variable Expansion ($) and Command Substitution ((), \``):** If you want to print a literal $` sign or a backtick, you           escape them.
    Bash

    echo "The cost is \$10."
    # Output:
    # The cost is $10.

    echo "Run a command: \$(date)" # To print literally $(date)
    # Output:
    # Run a command: $(date)

 6. Quoting vs. Escaping:

    Escaping (with \): Primarily used for single characters. It explicitly tells the shell to treat the next character literally.     It gives you very fine-grained control.

    Single Quotes (''): The strongest form of quoting. Everything inside single quotes is treated literally; no special               characters (including \ and $) are interpreted.
    Bash

   echo 'This is a string with $variables and \nnewlines and *wildcards.'
   # Output:
   # This is a string with $variables and \nnewlines and *wildcards.

 7. Double Quotes (""): A weaker form of quoting. Most special characters are treated literally, but variable expansion ($) and       command substitution ($(), `) are still performed. You still need to escape double quotes (\") and backslashes (\\)               themselves within double quotes.
    Bash

    my_var="value"
    echo "This is a string with $my_var and \nnewlines and *wildcards."
    # Output:
    # This is a string with value and \nnewlines and *wildcards.
