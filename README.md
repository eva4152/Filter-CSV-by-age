# Filter-CSV-by-age
In this program we are using different files by using different streams. We will use stdin, stdout and stderr. How we show the difference between stdout and stderr is by showing only the errors at stderr.
We firstly define or delimter, which in our case will be a ,. We then declare our pointer file variables, which will be initialzed based of our own input in the terminal. An arrar of chars is declared and initilized, which will be our info text.
The function filter_stream() we put our in and out file variable into the command-line interface. Then a while-loop will read a line from istream until theres no longer any lines from istream, by using the fgets function.
We then check our if our line and makes tokens of the first word at the line is assigned to name variables. and the newxt word after our delimeter is assign to the age, by using strtok.
If there isn't an age after, there we be printet an erorr message in stderr.
Also if there is no name, no word at all, another error message will be printet in stderr.
We the check our ages, and firstly we check if the age is an integer, if not, an erorr message will be printet in stderr. If it is an integer, we then check if our age is bigget than the max age, if true, in ostream will be printet the name and age.
In our main(), we put our userinputs arguments into a switchcase, and based of the number of arguments a different set apply. at the end theres a default case, where the info text is printet.
We will the try to open our in and out files, and make the ifile readabled, and the ofile writeable. we then call our filter_stream() function, where we put the users input into the commandline-interface.
