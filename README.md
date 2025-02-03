# Credit Card Fraud Detector

## Overview

Credit Card Fraud Detector is a system that identifies fraudulent transactions by monitoring credit card activity over a rolling 24-hour period. If the total amount of transactions for a specific card exceeds a predefined threshold, the card is flagged as fraudulent.

## Features
- Processes credit card transactions in real-time
- Uses a sliding 24-hour window to monitor activity
- Detects fraudulent transactions based on spending thresholds
- Supports input in CSV format

## Transaction Format
Each transaction consists of three elements:
- **Hashed Credit Card Number**
- **Timestamp** (format: `YYYY-MM-DDTHH:MM:SS`)
- **Amount** (format: `Dollars.Cents`)

Example:
```
10d7ce2f43e35fa57d1bbf8b1e2, 2014-04-29T13:15:54, 10.00
```

## Installation

### Prerequisites
- Java (JDK 8 or higher)
- Apache NetBeans (optional for development)
- Git (for version control)

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/CreditCardFraudDetector.git
   ```
2. Navigate to the project directory:
   ```sh
   cd CreditCardFraudDetector
   ```
3. Build the project using Apache NetBeans or run:
   ```sh
   javac -d bin src/**/*.java
   ```
4. Run the application:
   ```sh
   java -cp bin com.yourpackage.Main
   ```

## Usage
To analyze transactions, feed a CSV file containing transactions:
```sh
java -cp bin com.yourpackage.Main transactions.csv
```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a new feature branch
3. Commit changes and push to your fork
4. Submit a pull request


