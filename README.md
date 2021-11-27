# FP3-S01-Libraries-and-Modules
#Using already made arrays and breaking it up into modules and adding new functions


#Imports all modules from other codes
import addstudent
import removestudent
import printstudent
import savestudent

#Defines Student Marks to be used 
Student_Marks = {}


#How it works
print("""
This program makes a list of students and they're averages.
You can add students and there averages
Remove students
Print list
Save the infomration onto a text file
or exit
""")


go = True
while go == True:
    print("What do you want to do?")
    answear = input("Add, Remove, Print, Save, Exit. ")
    if answear == "add" or answear == "Add":
        Student_Marks = addstudent.addstudent(Student_Marks)
    elif answear == "remove" or answear == "Remove":
        removestudent.removestudent(Student_Marks)
    elif answear == "print" or answear == "Print":
        printstudent.printstudent(Student_Marks)
    elif answear == "save" or answear == "Save":
        savestudent.savestudent(Student_Marks)
    elif answear == "exit" or answear == "Exit":
        print("thanks, goodbye")
        go = False
    else:
        print("that is not an option")
        
        

        

        
        


