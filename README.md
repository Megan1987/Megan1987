# Megan1987

class Student(object):

    def __init__(self,name,gender):
        self.__name=name
        self.__gender=gender

    def set_gender(self,gender):
        if gender == 'male':
            self.__gender=gender
        elif gender == 'female':
            self.__gender=gender
        else:
            raise ValueError('Invalid')

    def get_gender(self):
        return self.__gender

Bart = Student('Bart', '3')
print(Bart._Student__name)
print(Bart.get_gender())

# the result still come out with below:
# Bart
# 3

# Where is wrong for the code?
