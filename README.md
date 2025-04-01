# Programming Patterns in Java and Python

> This document is a reference guide for core programming patterns used in beginner to intermediate level programming. Each pattern includes both **Java** and **Python** versions, with comments to explain what’s happening.

---

## 1. Sum Pattern

### Java
```java
// Calculate total rainfall using loop
double[] rainfall = {10, 11, 12, 9.5, 8.33};
double totalRainfall = 0;
for (int i = 0; i < rainfall.length; i++) {
    totalRainfall += rainfall[i];
}
System.out.println("Total Rainfall: " + totalRainfall);
```

### Python
```python
# Calculate total rainfall using built-in sum function
rainfall = [10, 11, 12, 9.5, 8.33]
totalRainfall = sum(rainfall)
print("Total Rainfall:", totalRainfall)
```

---

## 2. Output Pattern

### Java
```java
System.out.println("Age is " + age);
System.out.println("Name is " + name);
```

### Python
```python
print("Age is", age)
print("Name is", name)
# Or using f-strings
print(f"Age is {age}")
print(f"Name is {name}")
```

---

## 3. Input/Read Pattern

### Java
```java
System.out.print("Age: ");
int age = In.nextInt();
```

### Python
```python
age = int(input('Age: '))
```

---

## 4. Read Loop Pattern

### Java
```java
int card = In.nextInt();
while (card != -1) {
    sum += card;
    card = In.nextInt();
}
System.out.println("Total card value = " + sum);
```

### Python
```python
card = int(input('Enter card number: '))
while card != -1:
    sum += card
    card = int(input('Enter card number: '))
print("Total card value =", sum)
```

---

## 5. Count Pattern

### Java
```java
int count = 0;
for (int i = 0; i < profit.length; i++) {
    count++;
}
// With a guard
for (int i = 0; i < profit.length; i++) {
    if (profit[i] > 100)
        count++;
}
```

### Python
```python
count = 0
for i in range(len(profit)):
    count += 1
# With a guard
for i in profit:
    if i > 100:
        count += 1
```

---

## 6. Max Pattern

### Java
```java
double max = 0;
for (int i = 0; i < profit.length; i++) {
    if (profit[i] > max)
        max = profit[i];
}
```

### Python
```python
max1 = 0
for i in profit:
    if i > max1:
        max1 = i
# Python alternative
max1 = max(profit)
```

---

## ⭐ Next Steps

1. Save this file as `README.md`
2. Open VS Code and create a new folder `programming-patterns-notes`
3. Inside that folder, save this markdown file
4. Optional: Initialize a Git repo and push to GitHub:
```bash
git init
git add README.md
git commit -m "Initial commit: programming patterns"
git remote add origin https://github.com/YOUR-USERNAME/programming-patterns-notes.git
git push -u origin main
```

Happy coding! 🚀
