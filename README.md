# RoomReservation
This program implements a reservation system for booking time in a collection of rooms.  It provides the creation and deletion of reservations (on a single day), and prints information about the overall schedule. 
# Windows Compiler
This is for [Windows](https://msdn.microsoft.com/en-us/library/bb384838.aspx) users.
# Compiling and running multiple files with clang (OSX preferred way)
1. Open Terminal 
2. cd to the directory where the project is
3. clang -c -Wall -Werror -o m main.c
4. clang -c -Wall -Werror -o r rooms.c
5. clang -c -Wall -Werror -o s schedule.c
6. clang -o Program m r s
~~To run...~~
7. ./Program
# Compiling and running multiple files with GCC (Linux)
1. Open Terminal 
2. cd to the directory where the project is
3. gcc -c -Wall -Werror -o m main.c
4. gcc -c -Wall -Werror -o r rooms.c
5. gcc -c -Wall -Werror -o s schedule.c
6. gcc -o Program m r s
~~To run...~~
7. ./Program
# User interface and error handling
How many rooms?
\
Enter command (r,x,s,q): r 
\
=== MAKE RESERVATION ===
\
Enter name (one word): //There is a chunk of code that makes sure name does not exceed 20 chars the 20 chars can be //comprised of 
chars that are not letters so no ERROR checking for the actual characters
\
Start Time (hh:mm, 24-hr): //note: you do not need to have a 0 before a single digit hour for example 09:00 == 9:00 also if //you enter
something like Bob for the time DONT
\
End Time (hh:mm, 24-hr): //note: you do not need to have a 0 before a single digit hour for example 09:00 == 9:00 also if //you enter
something like Bob for the time DONT
\
//Also defualt opeining and closing times are 00:00 - 24:00 if you do something like 
\
Start Time (hh:mm, 24-hr): 24:00
End Time (hh:mm, 24-hr): 25:00 
\
//the reservation will be successful becuase there is no checking to see if the time passed is within the bounds of opening and closing
times this is something you have to make sure of









