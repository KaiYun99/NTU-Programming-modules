# Strong password require Uppercase, Lowercase, Digit and >= 8 Length

password = input("input your password:")
Uppercase = False
Lowercase = False
Digit = False

for b in password:
    if b.isupper():
        Uppercase = True
    if b.islower():
        Lowercase = True
    if b.isdigit():
        Digit = True
length = len(password)
lengths = 8
Strong = Uppercase and Lowercase and Digit and (length >= lengths) is True # Bracket is needed if not is "lengths is True"

if Strong:
    print("Your password is strong")
if not Strong:
    print("Your password is weak")
