# AcmeTravelPocMulesoft

## Mulesoft Project consuming ACME_Travel_POC API

The mule project is configured to listen on the machine's localhost:8081

getDestinationAirports
/destinationAirports/{pageNo}/{pageSize}/{name}

getFlightListByDate
/getFlights/{depDate}

simulateSeatPurchase
/simulateTicketPurchase/{flightId}/{depDate}

simulateNewSeatPrice
/amendFlightPrice/{flightId}/{depDate}/{newFlightPrice}

acmeTravelFlow
/insertNewFlight/{airlineId}/{sourceAirportId}/{destinationAirportId}/{departureDate}/{seatAvailability}/{price}
