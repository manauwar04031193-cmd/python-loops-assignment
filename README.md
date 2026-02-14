max_temp = temperatures[0]
min_temp = temperatures[0]
hot_days = 0

for t in temperatures:
    if t > max_temp:
        max_temp = t
    if t < min_temp:
        min_temp = t
    if t >= 32:
        hot_days += 1

print("Max:", max_temp)
print("Min:", min_temp)
print("Hot Days:", hot_days)

# Name: Manauwar Alam
# Roll Number: No
# Assignment: Python Loops & Automation - Subjective Question

print("===== Task 1: Find Maximum and Minimum =====")
temperatures = [28, 32, 35, 29, 31, 27, 30]

# Assume first value as max and min
max_temp = temperatures[0]
min_temp = temperatures[0]

for temp in temperatures:
    if temp > max_temp:
        max_temp = temp
    if temp < min_temp:
        min_temp = temp

print("Maximum Temperature:", max_temp)
print("Minimum Temperature:", min_temp)


print("\n===== Task 2: Count Hot Days =====")
temperatures = [28, 32, 35, 29, 31, 27, 30]

# Hot day = temperature >= 32
hot_days = 0

for temp in temperatures:
    if temp >= 32:
        hot_days += 1

print("Number of hot days:", hot_days)


print("\n===== Task 3: Alert System =====")
temperatures = [28, 32, 35, 40, 31, 33, 30]

for temp in temperatures:
    if temp >= 40:
        print("ALERT! Extremely Hot Day:", temp, "°C")
    elif temp >= 35:
        print("Warning! Very Hot Day:", temp, "°C")
    else:
        print("Normal Day:", temp, "°C")

