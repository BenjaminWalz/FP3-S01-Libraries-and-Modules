# FP3-S01-Libraries-and-Modules
#Using already made arrays and breaking it up into modules and adding new functions


def addstudent():
    Student_Marks = {}
    final_mark = 0
    number_marks = 0
    go = True
    newstudent = input("What is the name of the student? ")
    print("What are the marks of the student? Please give marks one at a time. Type 'done' when marks are entered")
    while go == True:
        marks = input("Marks > ").lower()
        if marks == 'done':
            go = False
        else:
            marks = int(marks)
            final_mark = marks + final_mark
            number_marks = number_marks + 1
    final_mark = final_mark / number_marks
    Student_Marks[newstudent] = final_mark
    print("You added", newstudent, "with an average of", final_mark)
    return Student_Marks
