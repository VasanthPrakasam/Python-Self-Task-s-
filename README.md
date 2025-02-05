# Python-Self-Task-
assigned by AI on the topic I refer And Please Guide me If I Am Wrong

Task 1 : is to assign the Donor based on the Blood group to the right counter using conditional Statement.

name = input("Enter name: ")
age = int(input("Enter age: "))
blood_group = input("Enter blood group: ").strip().upper()  # Standardizing input
# # The strip() function in Python is commonly used to remove any leading or trailing whitespace characters from a string. 
# In the context of your question, when you input a name, age, or blood group, 
# using strip() ensures that any accidental spaces before or after the input do not affect the final result.

# For example, if a user accidentally enters " John Doe " (with spaces), using strip() would convert it to “John Doe”, 
# which is cleaner and more consistent for further processing or storage. 
# Without strip(), the input would retain those spaces, potentially leading to issues in comparisons, data storage, or display.

# While the output may visually appear the same in some cases, the underlying data can differ significantly. 
# This can lead to unexpected behavior in applications, especially when performing operations like searching or matching strings. 
# Therefore, using strip() is a good practice to ensure data integrity and consistency.

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
