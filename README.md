# AcmeTravelPocMulesoft

## Mulesoft Project

The mule project is configured to listen on the machine's localhost:8081

The below requests can be sent to consume the ACME_Travel_POC

getDestinationAirports
http://localhost:8081/destinationAirports/{pageNo}/{pageSize}/{name}

getFlightListByDate
http://localhost:8081/getFlights/{depDate}

simulateSeatPurchase
http://localhost:8081/simulateTicketPurchase/{flightId}/{depDate}

simulateNewSeatPrice
http://localhost:8081/amendFlightPrice/{flightId}/{depDate}/{newFlightPrice}

acmeTravelFlow
http://localhost:8081/insertNewFlight/{airlineId}/{sourceAirportId}/{destinationAirportId}/{departureDate}/{seatAvailability}/{price}
