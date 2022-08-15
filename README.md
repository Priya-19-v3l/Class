from datetime import date
class Employee:
    def __init__(self,name,dob,salary,gender,city):
        self.name = name
        self.dob = dob
        self.salary = salary
        self.gender = gender
        self.city = city
        
    def address(self):
        addr = f'Name : {self.name}\nDOB : {self.dob}\nSalary : {self.salary}\nCity : {self.city}\nGender = {self.gender}'
        return addr
    
    
    def age(self):
        current_year=date.today().year
        return current_year - self.dob
    
emp1=Employee('Sangavi',1994,20000,'Female','Chennai')
emp2=Employee('Ragavan',1992,30000,'Male','Chennai')

print(emp1.address())
print(emp2.address())

print(emp1.age())
print(emp2.age())
        
