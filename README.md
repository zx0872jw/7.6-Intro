# 7.6-Intro
# Create the user input on line 3... user_input = input("Enter input string:\n")
user_input = input("Enter input string:\n")
while user_input != 'q':
    if user_input == 'q':
        break
    elif not ',' in user_input:
        print("Error: No comma in string.\n")
        user_input = input("Enter input string:\n")
    elif ',' in user_input:
        seperator = ','
        user_input1 = user_input.split(seperator)
        seperator1 = ' '
        user_input = seperator1.join(user_input1)
        user_input2 = user_input.split()
        print("First word:", user_input2[0])
        print("Second word:", user_input2[1])
        user_input = input("\nEnter input string:\n")
        

