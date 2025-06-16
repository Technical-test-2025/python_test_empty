# Test 2

## 🧪 Objective

Design a system to manage a fleet of vehicles for a rental company. The system should support different types of vehicles, each with specific attributes and behaviors.

## 📌 Requirements

### 1. Create a base class `Vehicle` with the following attributes:
- `brand` (string)
- `model` (string)
- `year` (integer)
- `mileage` (float)


Include the following methods:
- `display_info()` – returns a string with the vehicle's details.
- `drive(km)` – increases the mileage by the given number of kilometers.

### 2. Create the following subclass:
- `Car` – with an additional attribute `number_of_doors` (integer)

subclass should override the `display_info()` method to include its specific attributes.


### 3. Usage

- Create instances of `Car`` and demonstrate the functionality of the methods.
- In this code, which display_info method is called (Vehicle or Car class) ?
```python
    vehicle: Vehicle = Car(...)
    vehicle.display_info()
```
- What will be printed in the code below ?
```python
cars = [
    Car("Toyota", "Corolla", 2020, 15000.0, 4),
    Car("Honda", "Civic", 2019, 20000.0, 4)
]

# Get the first car and modify its brand
car = cars[0]
car2 = car
car2.brand = "Ford"
print(cars[0].display_info())


