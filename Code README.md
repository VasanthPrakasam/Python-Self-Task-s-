#Task 1 : is to assign the Donor based on the Blood group to the right counter using conditional Statement

name = input("Enter name: ")
age = int(input("Enter age: "))
blood_group = input("Enter blood group: ").strip().upper()  
# Standardizing input
# Assigning blood groups to respective counters
if blood_group == "A+":
    counter = 1
elif blood_group == "A-":
    counter = 2
elif blood_group == "B+":
    counter = 3
elif blood_group == "B-":
    counter = 4
elif blood_group == "O+":
    counter = 5
elif blood_group == "O-":
    counter = 6
elif blood_group == "AB+" or blood_group == "AB-":
    counter = 7
else:
    counter = "Invalid blood group"
# Display the assigned counter
if isinstance(counter, int):
    print(f"{name}, your blood group ({blood_group}) is assigned to Counter {counter}.")
else:
    print("Error: Please enter a valid blood group (A+, A-, B+, B-, O+, O-, AB+, AB-).")
