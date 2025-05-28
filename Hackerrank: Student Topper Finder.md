# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---

## 💻 PROGRAM:
```
n=int(input())
records={}

for _ in range(n):
    data=input().split()
    name,scores=data[0],list(map(float,data[1:]))
    records[name]=scores
    
query_name=input()
average=sum(records[query_name])/len(records[query_name])
print(f"{average:.2f}")
```

## OUTPUT
![image](https://github.com/user-attachments/assets/54d08cec-feb4-4a2e-bcce-d6b1392cc0e0)

## RESULT
Thus,the program is executed successfully
