# FlightBooking Smart Contract

## Overview
The **FlightBooking** smart contract provides a decentralized flight booking system built on the Ethereum blockchain. It allows airlines to create and manage flights, passengers to book and check in to flights, and users to leave reviews.

## Features
- **Flight Management:** Airlines can create, update, and delete flight details.
- **Seat Booking:** Passengers can book available seats.
- **Check-in:** Passengers can check in and trigger payments.
- **Refunds:** Passengers can cancel bookings and receive refunds.
- **Reviews:** Passengers can leave reviews for flights.
- **Secure Payments:** Funds are securely transferred using smart contracts.

## Technologies Used
- Solidity
- OpenZeppelin Libraries
  - Ownable
  - Counters
  - ReentrancyGuard

## Smart Contract Functions

### 🛫 **Flight Management**
- `createFlight`: Create a new flight.
- `updateFlight`: Update flight details.
- `deleteFlight`: Remove a flight.
- `getFlights`: Retrieve all active flights.
- `getFlight`: Get details of a specific flight.

### 🎟️ **Booking System**
- `bookFlight`: Book flight seats.
- `checkInFlight`: Check in to a booked flight.
- `refundBooking`: Cancel booking and receive refunds.

### ⭐ **Reviews**
- `addReview`: Add a review for a flight.

### 💸 **Payments**
- Payments are processed securely using `payTo`.

## Deployment
1. Clone the repository.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Compile the smart contract:
   ```bash
   npx hardhat compile
   ```
4. Deploy to a test network:
   ```bash
   npx hardhat run scripts/deploy.js --network goerli
   ```

## Security
- Reentrancy protection with OpenZeppelin's `ReentrancyGuard`.
- Owner privileges managed with `Ownable`.

## License
This project is licensed under the **MIT License**.

## Contact
- **Developer:** Uday Kiran Pedda
- **GitHub:** [udaykiranhub](https://github.com/udaykiranhub)
- **LinkedIn:** [Uday Kiran Pedda](https://www.linkedin.com/in/uday-kiran-pedda-65aa73271)

Feel free to contribute and improve this project!
