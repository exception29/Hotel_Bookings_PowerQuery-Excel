# Hotel_Bookings_PowerQuery-Excel
Input CSV files
1. bookings_data1: The bookings_data file consists of several columns, such as date, property_id, property_name, hotel_type, city|city_code, room_id, successful_bookings, and capacity. This file provides insights into the number of successful bookings made for a property on a given date and in a specific city, as well as the overall capacity of the property.

2. rooms_data: The rooms_data file consists of two columns, room_id and room_class. This file is useful in determining the room_class associated with each room_id in the bookings_data file.

- Performed Data Cleaning steps in Power Query to make data consistent.
- Created a new conditional column called "Availability Status". If "successful_bookings" equals "capacity", set the value to "sold out"; otherwise, set it to "vacant".
- Created a new custom column called "occ%", which represents the ratio of successful_bookings to capacity. 
- Merged the two tables, "bookings_data1" and "rooms_data", on the "room_id" column to add the "room_class" column to the "bookings_data" table.
