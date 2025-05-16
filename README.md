# FILE-HANDLING-UTILITY

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: CHALAKACHARLA CHANDU

*INTERN ID*: CT06DL1134

*DOMAIN*: FILE HANDLING UTILITY

*DURATION*: 6 WEEKS

*MENTOR*: NEELA SANTOSH

*DESCRIPTION*:

        The Java File Handling Utility program is designed to perform essential file operations, including writing, reading, and modifying text files. It uses core Java libraries for file handling, such as java.io.* for input and output operations and java.util.Scanner for user interaction. The program is structured with a main class named FileHandlingUtility, which contains three primary methods: writeToFile, readFromFile, and modifyFile. The purpose of these methods is to make file handling efficient, user-friendly, and interactive. The program also has a simple menu-driven interface to allow users to choose the desired operation.

The writeToFile method is responsible for adding content to a specified file. It uses BufferedWriter wrapped around FileWriter to efficiently write data to the file. The method opens the file in append mode, so any new content is added without erasing the existing data. This feature is useful when we need to keep a log or continuously update a file without losing previous entries. The program uses a try-with-resources block, which ensures that the file is automatically closed after writing, even if an error occurs. This approach helps prevent resource leaks and maintains efficient memory usage. If an error arises while writing to the file, an appropriate error message is displayed to inform the user.

Next, the readFromFile method handles reading the file content. It uses BufferedReader wrapped around FileReader to read data line by line, making it efficient for handling large text files. The method prints each line to the console, allowing users to view the entire content of the file. Just like the writing method, it uses the try-with-resources statement to manage resources effectively. If the file does not exist or cannot be accessed, the program catches the IOException and prints a descriptive error message. This method is particularly useful when the user wants to quickly view what is stored in a text file without manually opening it in an external editor.

The most complex part of the program is the modifyFile method, which allows users to replace specific text within the file. It reads the entire file content into a StringBuilder object, which is more memory-efficient than using plain strings, especially when dealing with large files. The method then performs a text replacement operation, changing all occurrences of the specified old string to the new one. Once the modification is complete, it writes the updated content back to the file. As with the other methods, it handles errors gracefully, informing the user if something goes wrong during reading or writing. This method is particularly useful when the user needs to update data or fix mistakes within a file.

The program's main method ties everything together by offering a simple text-based interface. After prompting the user to enter a file name, the program presents a menu with four options: write to file, read from file, modify file, and exit. Depending on the user’s choice, the corresponding method is called. This interactive approach makes it easy for users to perform file operations without needing advanced technical knowledge. Additionally, the program ensures that invalid inputs are handled correctly by displaying an error message when necessary. The program also closes the scanner properly before exiting to avoid resource leaks.

The program’s design is robust and practical. By incorporating error handling, it remains reliable even when encountering issues like missing files or incorrect input. The use of buffered I/O classes makes the program efficient, while the clear and straightforward code structure ensures that it is easy to understand and maintain. This utility can be useful for a variety of tasks, such as log management, updating configuration files, or processing text data. The flexibility of the code also allows it to be extended with additional features, such as deleting files or merging content from multiple files. Overall, this Java File Handling Utility demonstrates essential file operations with an interactive and user-friendly approach, making it a valuable tool for managing text files.
