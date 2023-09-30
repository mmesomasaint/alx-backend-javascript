# 0x02-ES6_classes

Trying to understand the basics of javascript `ES6` classes. This dir contains basic `beginners functions` and `code listings` to get you started.

## Topics

**Some topics here include:**

- [0-classroom.js](0-classroom.js)

  - Proper introduction to classes, declare a class `ClassRoom` with attributes.

- [1-make_classrooms.js](1-make_classrooms.js)

  - Create a function that returns an array of `ClassRoom` objects.

- [2-hbtn_course.js](2-hbtn_course.js)

  - Create a `HbtnCourse` class with attributes.
  - Verify the type of attributes during object creation.
  - Create a function that returns a `HbtnCourse` class.
  - Implement the `getter` and `setter` of each attribute.

- [3-currency.js](3-currency.js)

  - Create a `Currency` class with attributes.
  - Implement a method named `displayFullCurrency` that will return the attributes in the following format `name (code)`.
  - Implement the `getter` and `setter` of each attribute.

- [4-pricing.js](4-pricing.js)

  - Create a `Pricing` class with attributes.
  - Each attribute must be stored in an `underscore` attribute version (ex: `name` is stored in `_name`)
  - Implement a method named `displayFullPrice` that returns the attributes in the following format `amount currency_name (currency_code)`.
  - Implement the `getter` and `setter` of each attribute.
  - Implement a static method named `convertPrice`. It should accept two arguments: `amount` (Number), `conversionRate` (Number). The function should return the amount multiplied by the `conversion rate`.

- [5-building.js](5-building.js)

  - Create a `Building` class with attributes.
  - Each attribute must be stored in an `underscore` attribute version (ex: `name` is stored in `_name`)
  - Consider this class as an `abstract` class. And make sure that any class that extends from it should implement a method named `evacuationWarningMessage`.
    - If a class that extends from it does not have a `evacuationWarningMessage` method, throw an error with the message `Class extending Building must override evacuationWarningMessage`

- [6-sky_high.js](6-sky_high.js)

  - Create a `SkyHighBuilding` class that extends from `Building`.
  - Create a constructor with attributes.
  - Implement the `getter` and `setter` of each attribute.
  - Each attribute must be stored in an `underscore` attribute version (ex: `name` is stored in `_name`)
  - Override the method named `evacuationWarningMessage` and return the following string `Evacuate slowly the NUMBER_OF_FLOORS floors`.

- [7-airport.js](7-airport.js)

  - Create an `Airport` class with attributes.
  - Each attribute must be stored in an `underscore` attribute version (ex: `name` is stored in `_name`)
  - The default string description of the class should return the airport `code`.

- [8-hbtn_class.js](8-hbtn_class.js)

  - Create a `HolbertonClass` class with attributes.
  - Each attribute must be stored in an `underscore` attribute version (ex: `name` is stored in `_name`)
  - When the class is cast into a `Number`, it should return the size.
  - When the class is cast into a `String`, it should return the location.

- [9-hoisting.js](9-hoisting.js)

  - Fix this code and make it work.

  ```
  const class2019 = new HolbertonClass(2019, 'San Francisco');
  const class2020 = new HolbertonClass(2020, 'San Francisco');
  export class HolbertonClass {
  constructor(year, location) {
    this._year = year;
    this._location = location;
  }

  get year() {
    return this._year;
  }

  get location() {
    return this._location;
  }
  }
  const student1 = new StudentHolberton('Guillaume', 'Salva', class2020);
  const student2 = new StudentHolberton('John', 'Doe', class2020);
  const student3 = new StudentHolberton('Albert', 'Clinton', class2019);
  const student4 = new StudentHolberton('Donald', 'Bush', class2019);
  const student5 = new StudentHolberton('Jason', 'Sandler', class2019);
  export class StudentHolberton {
  constructor(firstName, lastName) {
    this._firstName = firstName;
    this._lastName = lastName;
    this._holbertonClass = holbertonClass;
  }

  get fullName() {
    return `${this._firstName} ${this._lastName}`;
  }

  get holbertonClass() {
    return this.holbertonClass;
  }

  get fullStudentDescription() {
    return `${self._firstName} ${self._lastName} - ${self._holbertonClass.year} - ${self._holbertonClass.location}`;
  }
  }
  export const listOfStudents = [student1, student2, student3, student4, student5];
  ```

- [10-car.js](10-car.js)

  - Implement a class named `Car` with constructor attributes.
  - Each attribute must be stored in an `underscore` attribute version (ex: `name` is stored in `_name`)
  - Add a method named `cloneCar`. This method should return a new object of the class.

- [100-evcar.js](100-evcar.js)

  - Implement a class named `EVCar` that extends the `Car` class (The class above).
  - Implement a constructor with attributes.
  - Each attribute must be stored in an `underscore` attribute version (ex: `name` is stored in `_name`)
  - For privacy reasons, when `cloneCar` is called on a `EVCar` object, the object returned should be an instance of `Car` instead of `EVCar`.
