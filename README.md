# Stock Market Trading System

A comprehensive C++ application that simulates a stock market trading environment with broker functionality, portfolio management, and real-time trading operations.

## 🚀 Features

- **Stock Management**: Create and manage stocks with unique IDs, names, prices, and volumes
- **User Portfolio**: Track stock holdings and available balance
- **Broker Services**: Enhanced trading with commission-based transactions
- **Market Operations**: Buy and sell stocks with real-time volume updates
- **Error Handling**: Comprehensive error checking for insufficient funds, stock availability, and portfolio validation
- **Interactive Interface**: Menu-driven console application for easy navigation

## 📋 Project Structure

```
Stock-Market-Trading-System/
├── code.cpp          # Main application source code
└── README.md         # Project documentation
```

## 🏗️ Architecture

### Core Classes

#### 1. **Stock Class**
- Manages individual stock information (ID, name, price, volume)
- Supports price updates and volume adjustments
- Handles stock display functionality

#### 2. **User Class**
- Base class for trading entities
- Manages portfolio (stock holdings)
- Handles balance tracking
- Provides buy/sell operations

#### 3. **Broker Class** (inherits from User)
- Enhanced user with commission-based trading
- Applies commission rates to both buy and sell operations
- Provides more realistic trading simulation

#### 4. **Market Class**
- Manages the collection of available stocks
- Provides stock lookup by ID
- Handles market display operations

## 🛠️ Requirements

- **C++ Compiler**: GCC 4.8+ or Visual Studio 2015+
- **C++ Standard**: C++11 or later
- **Operating System**: Windows, Linux, or macOS

## 🚀 Getting Started

### Compilation

#### Windows (using g++)
```bash
g++ -std=c++11 -o trading_system code.cpp
```

#### Linux/macOS
```bash
g++ -std=c++11 -o trading_system code.cpp
./trading_system
```

#### Visual Studio
1. Create a new C++ console project
2. Replace the default code with `code.cpp`
3. Build and run (Ctrl+F5)

### Running the Application

1. **Execute the compiled program**
2. **Enter initial broker balance** when prompted
3. **Set commission rate** (e.g., 0.02 for 2%)
4. **Navigate using the menu options**:
   - View Portfolio
   - Buy Stock
   - Sell Stock
   - View Market Stocks
   - Exit

## 📊 Default Stock Data

The system comes pre-loaded with popular tech stocks:

| Stock ID | Symbol | Price | Available Volume |
|----------|---------|-------|------------------|
| 1        | AAPL    | $150.00 | 1000 shares |
| 2        | GOOGL   | $2800.00 | 500 shares |
| 3        | AMZN    | $3500.00 | 300 shares |
| 4        | MSFT    | $380.00 | 800 shares |
| 5        | TSLA    | $250.00 | 600 shares |
| 6        | NVDA    | $900.00 | 400 shares |

## 🔧 Usage Examples

### Buying Stocks
1. Select option 2 (Buy Stock)
2. Enter Stock ID (1, 2, or 3)
3. Enter desired quantity
4. System validates funds and stock availability
5. Transaction processed with commission deduction

### Selling Stocks
1. Select option 3 (Sell Stock)
2. Enter Stock ID from your portfolio
3. Enter quantity to sell
4. System validates portfolio holdings
5. Transaction processed with commission applied

### Portfolio Management
- View current holdings and available balance
- Track stock quantities and values
- Monitor commission costs

## ⚡ Key Features

### Error Handling
- **Insufficient Balance**: Prevents purchases exceeding available funds
- **Stock Availability**: Validates stock volume before transactions
- **Portfolio Validation**: Ensures you own stocks before selling
- **Input Validation**: Handles negative values and invalid inputs

### Commission System
- Configurable commission rates for realistic trading
- Applied to both buy and sell operations
- Transparent commission calculation and display

### Dynamic Volume Management
- Real-time stock volume updates
- Prevents over-selling of available stocks
- Maintains market consistency

## 🎯 Future Enhancements

- [ ] Add more stock symbols and real-time price feeds
- [ ] Implement order types (market, limit, stop-loss)
- [ ] Add historical price tracking and charts
- [ ] Implement multi-user support
- [ ] Add database persistence
- [ ] Create GUI interface
- [ ] Add technical analysis indicators

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

Created as a demonstration of object-oriented programming concepts in C++ for stock market simulation.

---

**Happy Trading! 📈**