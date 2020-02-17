Description

    copy_text:
        This program is desgined to either take in an an extra 1 or 2 command prompts which are text files
        when running the code. When there is just the run command, it will read from stdin and print from stdout.
        If there is one extra command prompt, it will read the text file that was specified and output in one
        stdout. If there is two extra command prompts, the first text file specified will have their contents
        copied to the second.

    encode:
        ./encode - 
            when this command is entered alone. This will have the user enter in a string as long as 1024
            characters and indicate the end of the text with a lone '.' on a line. This will then automatically
            shift each letter by 13 if a shift size in not specified and output to stdout

        ./encode "shift_size" -
            when this command is entered, it will act like the first command however it will shift the letters
            by how much the shift was specified as

        ./encode "-F file.txt" -
            when this command is entered, this will open the file specified and output it to stdout. When -O
            is combined with the command, it will instead copy the text to the specified output text with a
            shift of 13 when a shift is not specified

        ./encode "-O file.txt"
            when this command is entered, this will have the user input a text and then once the text is complete
            indicating with a lone '.' on the last line, it will output the text to the specified text file or if
            there isn't one, it will create a new one. If a shift isn't specified it will shift it automatically
            by 13



Compiling the Code

	In the terminal, type in:
        make

Running the Code
    
	copy_text:
        ./copy "file_1.txt" "file_2.txt"
            /*the parameters after ./copy are optional if you do not include them it will just read and write from
            stdin and stdout*/
    
    encode:
        ./encode "shift" "-F file_1.txt" "-O file_2.txt"
            /*The parameters after ./encode are optional and the order of the three parameters can be ordered
            anyway the user wants as well as the '-' is not necessary for reading and writing parameters*/

Written By Trevor Le, Student ID: 1044055
