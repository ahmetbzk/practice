# Hi
[This is a google link](https://www.google.com/)
1. This is the first item
 1. This is a sub point
2. This is the second item

emphasis, aka italic, with

*asterisks* or _underscores_


strong is **double** or
scrate

~~~
import re
while True:
    name = input('Please enter your first name only \n').strip()

    if len(name) >= 1 and name.replace(' ','').isalpha():
        print ('Hello,'.capitalize(), name.capitalize())
        break
    else:
        print ('Please enter a valid name \n')


while True:
    password = input("Please enter a strong password with at least 8 character,\ncontain both uppercase and lowercase letters,\nhas atleast 1 number,\nand atleast 1 special character\n")
    if re.search(r"[A-Z]", password) is None:
        print("Password must have an uppercase letter\n")
    elif re.search(r"[a-z]",password) is None:
        print("Password must have a lowercase letter\n")
    elif len(password) < 8:
        print("Passowords must have 8 or more characters\n")
    elif re.search(r"[0-9]",password) is None:
        print("Password must have at least 1 number\n")
    elif re.search(r"[!@#$%^&*()_+{}:><?]", password) is None:
        print("Password must have at least 1 special character\n")
    else:
        print("Strong password", name, "Good Job")
        break
~~~
