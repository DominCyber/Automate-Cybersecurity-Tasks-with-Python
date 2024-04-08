# Automate Cybersecurity Tasks with Python
## Objective
Utilize the Coursera Google Cybersecurity Professional Certificate Course to obtain practical skills, like using Python-enabled to automate cybersecurity tasks. This course section provide guide projects to rapidly familiarize users with Python scripting fundamentals. Specifically, this project demonstrated processes that imported, opened, read, extracted, parsed, and updated data from an external log file, utilizing the various components of the Python Programming Language.

The project was presented as if the user was a security professional for a healthcare company who needed to vet an existing IP address allow list against a IP address remove list variable by running the allow list through a Python script.

### Skills Learned
-Understand how the Python programming language is used in security
<p>-Understand how various data types are handled in Python</p>
<p>-Incorporate variables into Python code</p>
<p>-Write conditional statements in Python</p>
<p>-Write iterative statements in Python</p>
<p>-Incorporate pre-built functions into code</p>
<p>-Create new, user-defined Python functions</p>
<p>-Understand how modules are used in Python</p>
<p>-Identify best practices to improve code readability</p>
<p>-Use Python to work with strings and lists</p>
<p>-Write simple algorithms</p>
<p>-Use regular expressions to extract information from text</p>
<p>-Use Python to automate tasks performed by security professionals</p>
<p>-Use Python to open and read the contents of a file</p>
<p>-Use Python to parse a file</p>
<p>-Practice debugging code</p>

### Tools Used
-Laptop
<p>-Coursera Google Cybersecurity Professional Certificate Course</p>

### Steps
<img src="https://i.imgur.com/7K0GFjR.jpg" style="width: 85%;" alt="1">
<p><i>Ref 1: Open, read, and convert the data type of the file that contains the allow list</i></p>
The variable "import_file" calls the stored text file that contains the allowed employee IP addresses.
The variable that contains the restricted IP addresses is included as well.
The OPEN function within the WITH statement contains the variable calling the file into the script as well as the “r” argument, all to store a working instance of the allow list file into memory with a reading execution into a variable called “file”.
From here, the “file” variable is passed off to a new variable, “ip_addresses”, in order to process the .read() function. Lastly, the “ip_addresses” variable is converted to a list data type with the .split() function, parsing the IP's out in a more readible format when passed off to the print() function.


<img src="https://i.imgur.com/60BcgsP.jpg" style="width: 85%;" alt="1">
<p><i>Ref 2: Iterative Statement writing</i></p>
After the .split() function is added, an FOR iterative statement is computed, which declares a new variable, “element”, which iteratively loops, throughout the data stored in “ip_addresses”, where the process is store therein. “Element” is passed off to the .print() function, demonstrating the execution of the  FOR statement.


<img src="https://i.imgur.com/MgYYP2p.jpg" style="width: 85%;" alt="1">
<p><i>Ref 3: Remove IP addresses that are on the remove list</i></p>
An IF conditional statement is added to the FOR iterative statement, which says that if there is any data found within the “remove_list” variable, when vetted against the stored data from “ip_addresses” in “element” an looped argument will evoke a .remove() function. This promptly removed data found in “remove_list”  from “ip_addresses”. This is ultimately passed on to the .print() function to output the allow list in the .split() function format, but noticably without the ip addresses found in “remove_list”.


<img src="https://i.imgur.com/76ZAuJ9.jpg" style="width: 85%;" alt="1">
<p><i>Ref 4: Update the file with the revised list of IP addresses</i></p>

Instead of printing an output, the newly updated data stored in “ip_addresses” is reformated with the .join function, followed by a WITH-OPEN statement denoting the agrument “w” (write) and “ip_addresses” stored within a new variable “file” which is passed off to to a .write() function, which ultimately updates the original “ip_addresses” memory space, and thus the external allow_list.txt file containing allowed employee host computer IP addresses which need access to patient PHI.
