This code implements a simple car rental system with three main classes: Car, Customer, and RentalAgency, along with a main class CarRentalSystem to run the system.

Car Class:
Represents a car available for rental.
Attributes:
make: String, the make of the car.
model: String, the model of the car.
year: int, the year of manufacture.
price: double, the rental price per day.
available: boolean, indicates if the car is available for booking.
Methods:
Car(String make, String model, int year, double price): Constructor to initialize a car object.
Getter methods for all attributes.
isAvailable(): Returns the availability status of the car.
setAvailable(boolean available): Sets the availability status of the car.
Customer Class:
Represents a customer who can book a car.
Attributes:
name: String, the name of the customer.
age: int, the age of the customer.
gender: String, the gender of the customer.
drivingLicense: String, the driving license number of the customer.
nationalID: String, the national ID number of the customer.
bookedCar: Car, the car booked by the customer.
Methods:
Customer(String name, int age, String gender, String drivingLicense, String nationalID): Constructor to initialize a customer object.
Getter methods for all attributes.
bookCar(Car car): Books a car for the customer.
RentalAgency Class:
Manages the rental agency operations.
Attributes:
cars: ArrayList<Car>, list of cars available for rental.
customers: ArrayList<Customer>, list of customers who have booked cars.
Methods:
RentalAgency(ArrayList<Car> cars): Constructor to initialize the rental agency with available cars.
getAvailableCars(): Retrieves a list of available cars.
bookCar(Car car, Customer customer): Books a car for a customer and adds the customer to the list of booked customers.
displayBookedCars(): Displays the list of booked cars along with the corresponding customers' names.
CarRentalSystem Class:
Main class to run the car rental system.
Methods:
main(String[] args): Entry point of the program.
displayAvailableCars(RentalAgency rentalAgency): Displays the list of available cars.
bookCar(RentalAgency rentalAgency, Scanner scanner): Books a car for the customer.
The main method in CarRentalSystem provides a menu-driven interface for users to view available cars, book a car, display booked cars, and exit the system.



