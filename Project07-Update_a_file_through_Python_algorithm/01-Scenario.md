SCENARIO:



You are a security professional working at a health care company. As part of your job, you're required to regularly update a file that identifies the employees who can access restricted content. The contents of the file are based on who is working with personal patient records. Employees are restricted access based on their IP address. There is an allow list for IP addresses permitted to sign into the restricted subnetwork. There's also a remove list that identifies which employees you must remove from this allow list.

Your task is to create an algorithm that uses Python code to check whether the allow list contains any IP addresses identified on the remove list. If so, you should remove those IP addresses from the file containing the allow list.





\# OPEN THE FILE THAT CONTAINS THE ALLOW LIST



The file that you want to open is called "allow\_list.txt". Assign a string containing this file name to the "import\_file" variable. Then, use a with statement to open it. Use the variable file to store the file while you work with it inside the with statement.





\# READ THE FILE CONTENTS



Next, use the .read() method to convert the contents of the allow list file into a string so that you can read them. Store this string in a variable called "ip\_addresses".





\# CONVERT THE STRING INTO A LIST



In order to remove individual IP addresses from the allow list, the IP addresses need to be in a list format. Therefore, use the .split() method to convert the "ip\_addresses" string into a list.





\# ITERATE THROUGH THE REMOVE LIST



A second list called "remove\_list" contains all of the IP addresses that should be removed from the "ip\_addresses" list. Set up the header of a for loop that will iterate through the "remove\_list". Use element as the loop variable.





\# REMOVE IP ADDRESSES THAT ARE ON THE REMOVE LIST



In the body of your iterative statement, add code that will remove all the IP addresses from the allow list that are also on the remove list. First, create a conditional that evaluates if the loop variable element is part of the "ip\_addresses" list. Then, within that conditional, apply the .remove() method to the "ip\_addresses" list and remove the IP addresses identified in the loop variable element.





\# UPDATE THE FILE WITH THE REVISED LIST OF IP ADDRESSES



Now that you have removed these IP addresses from the "ip\_address" variable, you can complete the algorithm by updating the file with this revised list. To do this, you must first convert the "ip\_addresses" list back into a string using the .join() method. Apply .join() to the string "\\n" in order to separate the elements in the file by placing them on a new line.

Then, use another with statement and the .write() method to write over the file assigned to the "import\_file" variable.





\# FINALIZE YOUT DOCUMENT



To finalize the document and make its purpose clear to potential employers, be sure to complete the Project description and Summary sections.

In the Project description section, give a general overview of the scenario and what you accomplished in Python.

In the Summary section, provide a short summary of the algorithm by highlighting its main components.

