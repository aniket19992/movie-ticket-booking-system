# movie-ticket-booking-system

Movie ticket booking app

Features:

Book Tickets
Show Status
Cancel Booking


Data Structure

A struct that behaves like a doubly linked list, it has values like

seat_no; -> Each row has seats from 1 to 9
row_no; -> Rows are from A to J
status; ->  make status'n' for not booked and 'b' for booked
*next; -> pointer to next seat
*prev; -> pointer to previous seat

We first create an object of class cinemax, we call the method obj.create(); to make a 2D array
of 10 rows from A to J and 9 columns from 1 to 9.

obj.display() method will print the 2D array of seat matrix for the user to see.

The user has 3 options to choose from here.

1. Book Ticket

To book tickets user enters the number of tickets to be booked, then he/she enters row and seat number of
all the tickets to be booked one by one. If invalid seat or row number is selected then appropriate error message is returned.
For all the booked tickets status is changed to 'b'.

There is a number variable that counts the total number of successfull tickets.

2. Show status

Just call obj.display() method to show the curent status of the seat matrix

3. Cancel booking

To cancel the booking of a given seat, user enters the row number and the seat number. The given row and seat no is found and if
its status is 'b' then its changed to 'n' else an error message is returned saying that UNBOOKED SEATS CANNOT BE CANCELLED.
