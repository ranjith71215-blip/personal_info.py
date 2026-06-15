# personal_info.py
Its a program that stores and displays personal information
print("=" * 50)
print("WELCOME TO MY PERSONAL INFORMATION PROGRAM")
print("=" * 50)


name = "Ranjith kumar"     
age = 20                
city = "bangalore"       
hobby = "Reading"      


age_in_months = age * 12


favorite_food = input("Enter your favorite food: ").strip()


while favorite_food == "":
    print("Favorite food cannot be empty. Please try again.")
    favorite_food = input("Enter your favorite food: ").strip()


favorite_color = input("Enter your favorite color: ").strip()


while favorite_color == "":
    print("Favorite color cannot be empty. Please try again.")
    favorite_color = input("Enter your favorite color: ").strip()


favorite_food = favorite_food.title()
favorite_color = favorite_color.title()


print("\n" + "=" * 50)
print("PERSONAL INFORMATION")
print("=" * 50)

print(f"Name           : {name.title()}")
print(f"Age            : {age}")
print(f"Age in Months  : {age_in_months}")
print(f"City           : {city.title()}")
print(f"Hobby          : {hobby.title()}")

print("-" * 50)
print("USER PREFERENCES")
print("-" * 50)

print(f"Favorite Food  : {favorite_food}")
print(f"Favorite Color : {favorite_color}")

print("=" * 50)
print("Thank you for using the Personal Information Program!")
print("Goodbye!")
