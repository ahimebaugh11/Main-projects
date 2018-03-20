# VariableIllustrator

Pass file path to create an object for a program file

FileInfo object will contain:
-printer() method prints contents of file linexline
-getFileLength() returns file length as an int
-getPath() returns path of the file as a string
-getFileContent() returns ArrayList<String> full of file contents arranged linexline
-remove(int z) removes from FileContent array the index of the int passed

Pass object to the intialization InitState class to run through the
array to find initialization statements, create an
object for each statement found

InitState object will contain:
-getInitLineNumArr() returns ArrayList of the initialization statements' line numbers
-getInitLineContents() returns ArrayList of the initialization statements' content linexline
-getInitLineNum(int x) returns the line number of the initialization statement specified
by index
-getInitLineContents() returns the line contents of the init statement specified by index


Pass InitState object and FileInfo object to UseLocator class to run through arrayList from FileInfo object to look
for other calls to the memory address present in InitInfo object. Creates an array from the line numbers of each memory
call then passes array, FileInfo, and InitInfo objects to Finalizer class, which will format and create a text file on
the desktop that holds all the relevant info

Finalizer Class:
-recieves FileInfo object
-recieves InitInfo object
-recieves lineNum array
-Formats and prints to a text file on the desktop
