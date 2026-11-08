# CyberSteps PowerShell Challenge – Part 1: Terminal Basics

**Challenge Completion Report**

As part of my CyberSteps Cybersecurity Analyst training, I successfully completed all 25 PowerShell challenges in Part 1: Terminal Basics.

The exercises helped me develop practical skills in navigating directories, managing files, working with variables, performing calculations, reading file contents, and using PowerShell pipelines.

During the challenges, I encountered several syntax errors, which helped me better understand the differences between PowerShell and Linux commands and how to troubleshoot incorrect commands.

## Completed Challenges – Commands and Explanations

1. **Hello, Terminal**
   `Write-Output "Hello, terminal"`
   Prints a text message to the console.

2. **The Console Is a Calculator**
   `Write-Output (8-4)`
   Performs a mathematical calculation and displays the result.

3. **The Answer to Everything**
   `Write-Output (6*7)`
   Multiplies two numbers and prints the result.

4. **Where Am I?**
   `pwd`
   Displays the current working directory.

5. **Spot the Doors**
   `Get-ChildItem -Directory -Name`
   Lists only folder names in the current directory.

6. **Peek Without Entering**
   `Get-ChildItem -Name storage`
   Lists the contents of the storage folder without entering it.

7. **Step Inside**
   `cd lab; Get-ChildItem -Name`
   Changes into the lab folder and lists its contents.

8. **Two Levels Down**
   `cd tools\scripts; pwd`
   Navigates two folder levels down and displays the current location.

9. **Up We Go**
   `cd bunker; cd ..; pwd`
   Enters the bunker folder, returns to the parent folder, and prints the location.

10. **Your First Variable**
    `$name = "Neo"; Write-Output $name`
    Stores a string in a variable and prints its value.

11. **Variables Can Do Math**
    `$numer1 = 10; $numer2 = 32; Write-Output ($numer1 + $numer2)`
    Stores two numbers in variables and calculates their sum.

12. **Build a Message**
    `$target = "server01"; Write-Output "Scanning $target"`
    Inserts a variable into a text message using string interpolation.

13. **Look Around**
    `Get-ChildItem -Name`
    Lists file and folder names without displaying additional details.

14. **Count the Loot**
    `(Get-ChildItem).Count`
    Counts the number of items in the current directory.

15. **Filter the Noise**
    `Get-ChildItem -Filter "*.txt" -Name`
    Displays only files matching the `.txt` extension.

16. **Read the Secret File**
    `Get-Content secret.txt`
    Reads and displays the contents of a text file.

17. **How Long Is the Log?**
    `@(Get-Content "log.txt").Count`
    Counts the number of lines in a text file.

18. **Find the Flag**
    `Get-ChildItem -Recurse -Filter "flag.txt" -File | Get-Content`
    Searches through subfolders for a specific file and displays its contents.

19. **Sort the Suspects**
    `Get-Content "names.txt" | Sort-Object`
    Reads names from a file and sorts them alphabetically.

20. **Tidy File List**
    `Get-ChildItem -File -Name | Sort-Object`
    Lists file names and sorts them alphabetically.

21. **Backwards, Please**
    `Get-Content "ranks.txt" | Sort-Object -Descending`
    Sorts the contents of a file in reverse alphabetical order.

22. **Variable Loot**
    `$file = "vault.txt"; Get-Content $file`
    Stores a filename in a variable and uses that variable to read the file.

23. **The Absolute Path**
    `Get-Content "C:\Users\khali\AppData\Local\Temp\CyberstepsPSQuest_Part1\sandbox\keys.txt"`
    Reads a file using its complete absolute path.

24. **Grand Finale**
    `cd logs; Get-ChildItem -Filter "*.log" -Name | Sort-Object`
    Enters the logs directory, filters `.log` files, and sorts their names alphabetically.

25. **Sign Off**
    `Write-Output "I am one with the shell"`
    Prints the final completion message.

## Conclusion

**Result: 25/25 Challenges Successfully Completed**

Through these exercises, I gained a better understanding of PowerShell command syntax, directory navigation, file operations, variables, and pipelines.

The most valuable learning experience was identifying and correcting syntax errors. I also learned how to combine multiple commands and use the pipeline operator (`|`) to process command output.

This practical training provides a foundation for further PowerShell scripting, system administration, and cybersecurity automation.
