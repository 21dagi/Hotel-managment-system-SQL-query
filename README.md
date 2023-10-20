# Hotel-managment-system-SQL-query
This is my sql query code for a hotel managment system
The provided SQL code creates several tables for a hotel management system:

The Hotel table stores information about hotels, such as the hotel ID, name, location, and phone number.

The Room table represents hotel rooms, with attributes like room ID, hotel ID (foreign key referencing the Hotel table), room type, price per night, and availability status.

The Reservable_table table is used to manage reservable tables in the hotel's restaurant or dining area. It includes attributes like table ID, table number, and floor number.

The Guest table stores details about hotel guests, including guest ID, first name, last name, gender, address, and phone number (unique).

The Reservation table tracks reservations made by guests. It includes reservation ID, guest ID (foreign key referencing the Guest table), room ID (foreign key referencing the Room table), reservable table ID (foreign key referencing the Reservable_table table), check-in and check-out dates, reservation status, and special requirements.

The CheckIn table captures check-in information for reservations. It includes a check-in ID (auto-incremented), reservation ID (foreign key referencing the Reservation table), check-in date and time, and room key.

The BestFoodDrink table represents the best food and drink items available in the hotel. It includes item ID, item name, and price.

The Order table tracks guest orders. It includes an order ID, guest ID (foreign key referencing the Guest table), item ID (foreign key referencing the BestFoodDrink table), and quantity.

The CheckOut table stores information related to guest check-outs. It includes checkout ID, reservation ID (foreign key referencing the Reservation table), order ID (foreign key referencing the Order table), checkout date and time, total cost, payment status, and checkout status.

These tables are designed to manage various aspects of a hotel management system, including hotels, rooms, reservations, check-ins, guest information, food and drink orders, and check-outs
