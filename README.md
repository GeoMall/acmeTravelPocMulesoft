# AcmeTravelPocMulesoft

## Mulesoft Project

The mule project is configured to listen on the machine's localhost:8081

The below requests can be sent to consume the ACME_Travel_POC:

### getDestinationAirports
This flow sends a request to the ACME Travel API by consuming the get method `acmeTravel/destinationAirports`. This flow is invoked when the link `http://localhost:8081/destinationAirports/{pageNo}/{pageSize}/{name}` is accessed. It needs the page number, page size and name parameters to be passed inorder to get a paginated list of the destination airports.

### getFlightListByDate
This flow sends a request to the ACME Travel API by consuming the get method `acmeTravel/flights`. This flow is invoked when the link `http://localhost:8081/getFlights/{depDate}` is accessed. It needs the departure date, in the form of *yyyy-MM-dd HH:mm:ss* or *yyyy-MM-dd* patterns, to be passed to get the flight list of that particular date.

### simulateSeatPurchase
This flow sends a request to the ACME Travel API by consuming the patch method `acmeTravel/simulateTicketPurchase`. This flow is invoked when the link `http://localhost:8081/simulateTicketPurchase/{flightId}/{depDate}` is accessed. It needs the flight Id and departure date, in the form of *yyyy-MM-dd HH:mm:ss* or *yyyy-MM-dd* patterns, to be passed to decrease the seat availability of that particular flight.

### simulateNewSeatPrice
This flow sends a request to the ACME Travel API by consuming the patch method  `amceTravel/amendFlightPrice`. This flow is invoked when the link `http://localhost:8081/amendFlightPrice/{flightId}/{depDate}/{newFlightPrice}` is accessed. It needs the flight Id, departure date, in the form of *yyyy-MM-dd HH:mm:ss* or *yyyy-MM-dd* patterns, and the new flight price to be passed to change the seat price of that particular flight.

### insertNewFlight
This flow sends a request to the ACME Travel API by consuming the post method `amceTravel/insertNewFlight`. This flow is invoked when the link `http://localhost:8081/insertNewFlight/{airlineId}/{sourceAirportId}/{destinationAirportId}/{departureDate}/{seatAvailability}/{price}` is accessed. It needs the airline Id, source airport Id, destination airport Id, departure date, in the form of *yyyy-MM-dd HH:mm:ss* or *yyyy-MM-dd* patterns, seat availability and price to be passed to create a new flight.
