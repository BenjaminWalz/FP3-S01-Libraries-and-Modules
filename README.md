# FP3-S01-Libraries-and-Modules
#Using already made arrays and breaking it up into modules and adding new functions


def savestudent(Student_Marks):
    print("What do you want to name your save?")
    save_name = input("> ")
    save_name = save_name + '.txt'
    save = open(save_name, 'w')
    saved_marks = str(Student_Marks)
    save.write(saved_marks)
