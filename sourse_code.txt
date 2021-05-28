def getdate():
    import datetime
    return datetime.datetime.now()

                                                # LOGING DATA
def log_data():
    print("Whose client data you want to log:\n1.Harry\n2.Hamad\n3.Rohan")
    num2 = int(input(":-"))
    # loging harry data
    if (num2 == 1):
        print("What you want to log in harry's data:\n1.Food\n2.exercise")
        num3 = int(input(":-"))
        if (num3 == 1):
            with open("exercise_5_food_harry.txt", "a") as file:
                food = input("Enter food:")
                file.write("[" + str(getdate()) + "]:"+food + "\n")
                print("___Successfully entered___")
        elif (num3 == 2):
            with open("exercise_5_exercise_harry.txt", "a") as file:
                exercise = input("Enter exercise:")
                file.write("[" + str(getdate()) + "]:"+exercise + "\n")
                print("___Successfully entered___")
    # loging hamad data
    elif (num2 == 2):
        print("What you want to log in hamad's data:\n1.Food\n2.exercise")
        num3 = int(input(":-"))
        if (num3 == 1):
            with open("exercise_5_food_hamad.txt", "a") as file:
                food = input("Enter food:")
                file.write("[" + str(getdate()) + "]:"+food + "\n")
                print("___Successfully entered___")
        elif (num3 == 2):
            with open("exercise_5_exercise_hamad.txt", "a") as file:
                exercise = input("Enter exercise:")
                file.write("[" + str(getdate()) + "]:"+exercise + "\n")
                print("___Successfully entered___")
    # loging rohan data
    elif (num2 == 3):
        print("What you want to log in rohan's data:\n1.Food\n2.exercise")
        num3 = int(input(":-"))
        if (num3 == 1):
            with open("exercise_5_food_rohan.txt", "a") as file:
                food = input("Enter food:")
                file.write("[" + str(getdate()) + "]:"+food + "\n")
                print("___Successfully entered___")
        elif (num3 == 2):
            with open("exercise_5_exercise_rohan.txt", "a") as file:
                exercise = input("Enter exercise:")
                file.write("[" + str(getdate()) + "]:"+exercise + "\n")
                print("___Successfully entered___")

                                                # RETRIVING DATA
def retrive_data():
    print("Whose client data you want to retrive:\n1.Harry\n2.Hamad\n3.Rohan")
    num4 = int(input(":-"))
    # retriveing harry data
    if (num4 == 1):
        print("Harry's which data you want to retrive:\n1.Food\n2.Exercise")
        num5 = int(input(":-"))
        if (num5 == 1):
            with open("exercise_5_food_harry.txt", "r") as file:
                print(file.read())
        elif(num5==2):
            with open("exercise_5_exercise_harry.txt","r")as file:
                print(file.read())
    # retriveing hamad data
    elif (num4 == 2):
        print("Hamad's which data you want to retrive:\n1.Food\n2.Exercise")
        num5 = int(input(":-"))
        if (num5 == 1):
            with open("exercise_5_food_hamad.txt", "r") as file:
                print(file.read())
        elif (num5 == 2):
            with open("exercise_5_exercise_hamad.txt", "r")as file:
                print(file.read())
    # retriveing rohan data
    elif (num4 == 3):
        print("Rohan's which data you want to retrive:\n1.Food\n2.Exercise")
        num5 = int(input(":-"))
        if (num5 == 1):
            with open("exercise_5_food_rohan.txt", "r") as file:
                print(file.read())
        elif (num5 == 2):
            with open("exercise_5_exercise_rohan.txt", "r")as file:
                print(file.read())

print("What you want to do\n1.log data\n2.retrive data")
num1 = int(input(":-"))
if (num1 == 1):
    log_data()
elif (num1 == 2):
    retrive_data()
