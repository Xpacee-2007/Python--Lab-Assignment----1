# Python--Lab-Assignment----1

# =========================
# LISTS
# =========================

# Lists are ordered, mutable, and allow duplicate values in Python.

students = ["Abhiraj", "Sumedh", "Kushagra", "Vaidic", "Naman", "Aadidev", "Sehajveer"]

# Adds "not a student" to the end of the list
students.append("not a student")
print(students)

# Removes the last item from the list
# pop() can also remove a specific index, e.g. students.pop(2)
students.pop()
print(students)

# Sorts the list in alphanumeric order (ascending)
students.sort()
print(students)

# Reverses the order of the list
students.reverse()
print(students)

# Copies the list
classmates = students.copy()
print(classmates)


# =========================
# TUPLES
# =========================

# Tuples are ordered, immutable, and allow duplicate values.

car_brand = (
    "Mercedes",
    "Audi",
    "Volvo",
    "BMW",
    "Maserati",
    "Porsche",
    "BMW",
    "Honda",
    "Mercedes",
    "Maserati",
    "Bugatti",
    "Honda",
    "Honda"
)

# Gives the number of times "Honda" appears
print(car_brand.count("Honda"))

# Gives the index of the first occurrence of "Maserati"
print(car_brand.index("Maserati"))

# Gives the length of the tuple
print(len(car_brand))


# =========================
# TUPLE UNPACKING
# =========================

(
    green,
    yellow,
    red,
    violet,
    blue,
    orange,
    indigo,
    pistacio,
    pink,
    brown,
    black,
    purple,
    hotpink
) = car_brand

print(green)
print(yellow)
print(red)
print(violet)
print(blue)
print(orange)
print(indigo)
print(pistacio)
print(pink)
print(brown)
print(black)
print(purple)
print(hotpink)


# =========================
# JOINING TUPLES
# =========================

tyres = (
    "Michelin",
    "Pirelli",
    "Bridgestone",
    "Continental",
    "MRF"
)

# Joins two tuples using +
tyres_shop = car_brand + tyres
print(tyres_shop)


# =========================
# DICTIONARIES
# =========================

# Dictionaries store data in key:value pairs.
# They are ordered, mutable, and do not allow duplicate keys.

car_shop = {
    "Car_Model": "M5",
    "Brand": "BMW",
    "tires": "pirelli",
    "color": "blue"
}

# Displays all the keys
print(car_shop.keys())

# Displays all the values
print(car_shop.values())

# Displays all key:value pairs
print(car_shop.items())

# Changes the value of "color"
car_shop["color"] = "black"
print(car_shop)

# The same thing can also be done using update()
car_shop.update({"color": "black"})
print(car_shop)
