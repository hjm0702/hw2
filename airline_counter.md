# Airline Ticket Agent

<img width="600px" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1c/Salt_Lake_City_-_Ticket_Counter_%2828301627663%29.jpg/1599px-Salt_Lake_City_-_Ticket_Counter_%2828301627663%29.jpg">


In this scenario, you will build an application for
an airline ticket agent at O'Hare.  Customers arrive at the airport
and expect to be able to perform the following transactions
with the ticket agent:

* Buy a one-way ticket for a flight
* Get a refund for a ticket whose flight has not yet departed
* Check the status of a ticket they've already purchased

Therefore, a ticket agent needs to:

* Get a list of flights for any given date, up to 30 days in advance
* Sell a new, one-way ticket for any flight up to 30 days in advance
* Lookup a ticket given a ticket number
* Refund a ticket when presented at the counter, if the flight
has not departed yet
* Given a date and a destination city, find out how many seats
remain and their prices.

The system should:

* Make sure every ticket has a unique identifier
* Prevent refunds from being given for flights that have already
departed
* Dynamically determine the price for a ticket based on factors
such as the row number and the percentage of seats already sold

Business Rules:

* The airline only sells one-way tickets.
* The application will only sell tickets leaving O'Hare.
* The airline serves five other cities.
* There are five flights per day: one flight to each city.
* Each airplane has 100 seats.
* Each airplane has 25 rows.
* Ticket prices are determined automatically by the system.
* The lowest possible ticket price is $100.
* The highest possible ticket price is $200.
* At any given time, the lower the row number, the higher the price
  will be for vacant seats. Alternatively, rows can be grouped into
  cabins in which all rows within a class cost the same; but
  cabins closer to the front of the plane must cost more than
  cabins toward the back.
* At any given time, ticket prices should vary directly with the
  percentage of vacant seats.  The fewer vacant seats there are,
  the higher the price should be for all vacant seats.
