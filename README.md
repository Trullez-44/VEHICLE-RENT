# README - Vehicle Rental Management

#### Welcome to the documentation of the vehicle rental management database! I'll explain how the tables work and what data they store.

## Conceptual Data Model - Vehicle Rental Management
#### In this conceptual data model, we describe the main entities and their relationships for vehicle rental management. The entities are:

## CUSTOMERS
The `CUSTOMERS` table stores information about customers. Each customer has a unique ID, and details such as name, last name, date of birth, address, phone number, email, and driver's license are recorded.
   - Attributes: ID, Name, Last Name, Date of Birth, Address, Phone, Email, Driver's License.
   - Relationships: A customer can make multiple rentals.

## VEHICLES
The `VEHICLES` table manages information about the vehicles available for rent. Each vehicle has a unique ID, and data such as the license plate, range, insurance status, vehicle status, brand, and model are stored.
   - Attributes: ID, Plate, Range, Insurance, Vehicle Status, Brand, Model.
   - Relationships: Multiple rentals can be associated with a vehicle. Each vehicle has a recorded status.


## DROP-OFFS
The `DROP-OFFS` table records information about vehicle returns. It includes the return ID, date and time of the return, vehicle condition at return, and whether the return was on time.
   - Attributes: ID, Drop-Off Date and Time, Vehicle Condition at Drop-Off, Punctuality.
   - Relationships: Multiple rentals can have associated drop-offs.

## RECORDS
The `RECORDS` table is used to document rental details. It includes a unique ID, related rental and return IDs, the payment method used, information about penalties, and other relevant details.
   - Attributes: ID, Details, Penalty.
   - Relationships: A record is related to a rental, a drop-off, and a payment method.

## PAY-METHOD
The `PAY-METHOD` table stores information about payment methods. Each customer has a registered payment method, which can be cash or card, with details such as card number, CVV, cardholder name, and expiration date.
   - Attributes: Payment Method (Cash, Card), Card Number, CVV, Cardholder Name, Expiration Date.
   - Relationships: Each customer has a registered payment method.

## VEHICLE-STATUS
The `VEHICLE-STATUS` table tracks the status of vehicles. It includes the vehicle ID, information on whether it is new, the mileage, and details about any damages.
   - Attributes: Status (New or Not New), Mileage, Damages.
   - Relationships: Each vehicle has a recorded status.

## RENTALS
The `RENTALS` table records rental information. Each rental has a unique ID, with details about the customer, vehicle, start and end dates of the rental, and other critical information.
   - Attributes: ID, Start Date, End Date, Details.
   - Relationships: Each rental is associated with a customer and a vehicle.

##### This conceptual model provides a high-level view of the key entities and the relationships between them in the vehicle rental management system. Each entity represents an important part of the database and how they relate to each other. This model serves as a solid foundation for creating more detailed logical and physical models.

### Physical Data Model - Vehicle Rental Management

##### The physical data model is a detailed representation of how the database is implemented in a specific database management system. It defines the physical structures, including tables, columns, data types, and constraints. This model is used for creating and maintaining the actual database in a database management system.

##### Below, you'll find an image depicting the physical data model of the vehicle rental management database. This image visually illustrates the table structures and their relationships within the database:

![Descripción de la imagen](/IMGS/VEHICLE_RENT.png)

### I hope this explanation helps you understand how the data is structured and related in this database! If you have any questions or need further assistance, please don't hesitate to contact me.

Trullez-44

@CAMPUSLANDS
