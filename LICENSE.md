def sort_students(students):
    students.sort(key=lambda student: student.cgpa, reverse=True)
class Student:
    def __init__(self, name, roll_number, cgpa):
        self.name = name
        self.roll_number = roll_number
        self.cgpa = cgpa

# Creating a list of student objects
students = [
    Student("John", "A001", 3.8),
    Student("Alice", "A002", 3.9),
    Student("Bob", "A003", 3.7),
    Student("Eve", "A004", 3.5)
]

# Sorting the list of students based on CGPA
sort_students(students)

# Printing the sorted list of students
for student in students:
    print(f"Name: {student.name}, Roll Number: {student.roll_number}, CGPA: {student.cgpa}")
