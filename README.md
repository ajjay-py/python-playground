## python-playground
My personal playground for learning, experimenting, and building with Python.

#practice date-2 Aug 2026#
#Return value - in function
def get_formatted_name(f_name, l_name):
    """Return full formatted name, neatly."""
    full_name = f"{f_name} {l_name}"
    return full_name.title()

musician = get_formatted_name('jimi', 'hendrix')
print(musician)

##None default
def build_persion(f_name, l_name, age=None):
    """Return a dictionary of info about a person"""
    person = {'first': f_name, 'last': l_name}
    if age:
        person['age'] = age
    return person

musician = build_persion('ajay', 'rathore', age=35)
print(musician)

#### using a function with a while loop
#using a function with while loop #
def get_formatted_name(f,l):
    """return a fully name with neatly"""
    full_name = f"{f} {l}"
    return full_name.title()

#This is a infinite loop
while True:
    print("\nPlease tell me your name:")
    print("(enter 'q' at any time to quit)")

    f = input("first name: ")
    if f == 'q':
        break
    l = input("last name: ")
    if l == 'q':
        break

    formatted_name = get_formatted_name(f,l)
    print(f"\nHello {formatted_name}")


    ##CITY DETAILS###
    def city_country(c_name , country):
    """Details about city and country."""
    city_detail = f'"{c_name},{country}"'
    return city_detail.title()

c_detail = city_country('pune', 'india')
print(c_detail)

#######Date: 3-AUG-2026 ##############
def greet_user(names):
    """Print a simple greet message to user."""
    for name in names:
        msg = f"Hello, {name.title()}!"
        print(msg)

usernames = ['sam','pam','jam']
greet_user(usernames)
