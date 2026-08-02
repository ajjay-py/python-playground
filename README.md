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
