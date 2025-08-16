# Flight Prices

![Airplane](Image/AIRPLANE.jpg)

---

This dataset is a CSV file where each row is a purchasable ticket found on Expedia between **2022-04-16** and **2022-10-05**, to/from the following airports:  
`ATL, DFW, DEN, ORD, LAX, CLT, MIA, JFK, EWR, SFO, DTW, BOS, PHL, LGA, IAD, OAK`.

---

## ❓ Question
**What is the lowest price from the top airport?**

---

## 📑 Content
- **legId**: An identifier for the flight.  
- **searchDate**: The date (YYYY-MM-DD) on which this entry was taken from Expedia.  
- **flightDate**: The date (YYYY-MM-DD) of the flight.  
- **startingAirport**: Three-character IATA airport code for the initial location.  
- **destinationAirport**: Three-character IATA airport code for the arrival location.  
- **fareBasisCode**: The fare basis code.  
- **travelDuration**: The travel duration in hours and minutes.  
- **elapsedDays**: The number of elapsed days (usually 0).  
- **isBasicEconomy**: Boolean for whether the ticket is for basic economy.  
- **isRefundable**: Boolean for whether the ticket is refundable.  
- **isNonStop**: Boolean for whether the flight is non-stop.  
- **baseFare**: The price of the ticket (in USD).  
- **totalFare**: The price of the ticket (in USD) including taxes and other fees.  
- **seatsRemaining**: Integer for the number of seats remaining.  
- **totalTravelDistance**: The total travel distance in miles (sometimes missing).  
- **segmentsDepartureTimeEpochSeconds**: Departure time (Unix time) for each leg, separated by `||`.  
- **segmentsDepartureTimeRaw**: Departure time (ISO 8601 format) for each leg, separated by `||`.  
- **segmentsArrivalTimeEpochSeconds**: Arrival time (Unix time) for each leg, separated by `||`.  
- **segmentsArrivalTimeRaw**: Arrival time (ISO 8601 format) for each leg, separated by `||`.  
- **segmentsArrivalAirportCode**: Arrival airport code for each leg, separated by `||`.  
- **segmentsDepartureAirportCode**: Departure airport code for each leg, separated by `||`.  
- **segmentsAirlineName**: Airline name for each leg, separated by `||`.  
- **segmentsAirlineCode**: Two-letter airline code for each leg, separated by `||`.  
- **segmentsEquipmentDescription**: Airplane type (e.g. Airbus A321, Boeing 737-800), separated by `||`.  
- **segmentsDurationInSeconds**: Flight duration in seconds for each leg, separated by `||`.  
- **segmentsDistance**: Distance traveled (in miles) for each leg, separated by `||`.  
- **segmentsCabinCode**: Cabin code (e.g. "coach") for each leg, separated by `||`.  

---

## 📝 Problem Statement
Our purpose is to use the data to **find the lowest price from the top airport**:  
1. Identify the airport with the highest number of departures.  
2. Find the minimum ticket price among all flights departing from that airport.  

---

## 📊 Data Description
The dataset was downloaded from Kaggle:  
🔗 [Flight Prices Dataset](https://www.kaggle.com/datasets/dilwong/flightprices/data)

---

## ⚙️ Algorithm
We will:
1. Build different **classification models**.  
2. Choose the best model based on **classification metrics**.  
3. Apply **feature engineering** to enhance model performance.  

---

## 🛠️ Tools
- **Technologies**: Python, Jupyter Notebook.  
- **Libraries**: NumPy, Pandas, Sklearn, Matplotlib, Seaborn, Tableau.  
