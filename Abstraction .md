# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program

```
from abc import ABC,abstractmethod
class type_shape(ABC): 
    @abstractmethod
    def area(self):
        pass

class Rectangle(type_shape):
  length = 6
  breadth = 4
  def area(self):
    return self.length * self.breadth

class Circle(type_shape):
  radius = 7
  def area(self):
      return 3.14*self.radius*self.radius

r = Rectangle() 
c = Circle() 
print("Area of a rectangle:", r.area()) 
print("Area of a circle:", c.area())

```

## Output
![Screenshot 2025-05-23 143830](https://github.com/user-attachments/assets/92285e53-4be6-4ff9-8580-51f7d4c2e2d5)



## Result
A python program with an **abstract class** named `Shape` with an **abstract method** `calculate_area`, is successfully implemented in two subclasses: `Rectangle` and `Circle`.
