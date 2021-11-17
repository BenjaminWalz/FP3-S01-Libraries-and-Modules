# FP3-S01-Libraries-and-Modules
#Using already made arrays and breaking it up into modules and adding new functions


def removestudent(Student_Marks):
    go = True
    print("What student do you want to remove? Type 'done' when student is removed. ")
    while go == True:
        student = input("Student> ")
        if student == 'done' or student == 'Done':
            go = False
        elif student in Student_Marks:
            print("You removed", student)
            del Student_Marks[student]
            go = False
        else:
            print("That student is not in the list")
        return Student_Marks
