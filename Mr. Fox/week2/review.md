# WEEK 2

## Something left behind
1. Better data format for dict file:
Apple - fruit
Rose - flower

2. DO NOT do regular logic in 'finally' statement. It is normally used to release resources ONLY.
  - More specifically, finally statement should NEVER throw another exception, therefore we usually don't put much logic into it.

3. Logical bugs:
  - Run the application -> wait for 5 min -> add new line in dict (e.g Bug -> something wrong in a program) -> test with the new word -> not working

4. Exception handling
  - When something unexpected ongoing, DO NOT pretend everything is fine by printing an 'Unknown'. Print error instead.

5. Why we need 3 timestamps? (local_time, st_mtime, last_time_filechange). Looks quite messy.


## New features to add
1. A new command 'load' enables it load another dict file by inputting 'load -file file2.txt'.
2. Timer for the command 'load'.
3. The in-memory dict need to COMBINE all the records from files it loaded.
4. The records with the same key NEVER OVERRIDE each other.
  e.g. File1.txt: Apple - Fruit
       File2.txt: Apple - Sweet
       -----
       load -file File1.txt
       load -file File2.txt
       Apple -> Fruit (NOT Sweet)

## Think 
1. How to avoid repeating similar|same logic in the code.
2. How to group & maintain the code by features.




