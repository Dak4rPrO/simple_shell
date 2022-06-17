# Simple_SHELL
- ## In this project I design a "Basic-Shell" applying most of the topics that I have learned during my first 3 months of programming.

Small summary of how my simple-shell works:

- Waits for user input
- Analyze the input (Receive command)
- Defines what type of command it is (what arguments it has, if it has pipe or redirection)
- Look for the command in the PATH or in the files (depending on which command it is)
- Call the default function of that command
- Return the result

The syntax would be the following:

	      1	          2		   3                   4
	command name {arguments} {pipe or redirection} {others arguments}

For example:

	 1   2    3       4
	ls {-l } {>} {file_name}

In the main function of my simple-shell there are the following calls.

- Fork
- Wait
- Pid
