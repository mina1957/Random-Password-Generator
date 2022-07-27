from curses.ascii import isdigit
import random
#Function checks if input is numeric
def numeric_check(input):
    for i in range(len(input)):
        if not isdigit(input[i]):
            return False
    return True

#Setting all characters to be used in password 
upper_case_letters = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
lower_case_letters = "abcdefghijklmnopqrstuvwxyz"
digits = "1234567890"
special_characters = "@#$%&*+=-_!"
all_chars = upper_case_letters + lower_case_letters + digits + special_characters

#Getting length of password from user
length_password = input("Desired password length: ")

#Checks if user input is valid
while  not numeric_check(length_password):
    print("\nPlease enter a number!\n")
    length_password = input("Desired password length: ")

#Generating random password
password = "".join(random.sample(all_chars, int(length_password)))

#Print generated password
print("Generated password: ", password)
