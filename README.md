# Age Calculator

A simple and intuitive web-based age calculator that computes your exact age in years, months, and days based on your birth date. Built with vanilla JavaScript, HTML, and CSS for optimal performance and accessibility.

## Features

- **Precise Age Calculation**: Calculate exact age down to the day
- **Real-time Updates**: Instantly displays results as you input your birth date
- **User-friendly Interface**: Clean, responsive design that works on all devices
- **Input Validation**: Prevents invalid dates and future dates
- **Multiple Date Formats**: Supports various date input methods
- **Zero Dependencies**: Built with vanilla JavaScript for fast loading

## Getting Started

### Prerequisites

No special requirements needed. This application runs in any modern web browser with JavaScript enabled.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/chstridho/age-calculator.git
   ```

2. Navigate to the project directory:
   ```bash
   cd age-calculator
   ```

3. Open `index.html` in your web browser or serve it through a local web server.

### Local Development

For local development, you can use any static file server. Here are a few options:

**Using Python (if installed):**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Using Node.js (if installed):**
```bash
npx serve .
```

Then visit `http://localhost:8000` in your browser.

## Usage

1. Enter your birth year in the year field (4-digit format)
2. Select or enter your birth month (1-12)
3. Enter your birth day (1-31, validated based on the selected month)
4. Your exact age will be calculated and displayed automatically
5. The result shows your age in years, months, and days

### Example

If today is August 21, 2025, and you were born on January 15, 1990, the calculator will display:
- **Age**: 35 years, 7 months, and 6 days

## File Structure

```
age-calculator/
│
├── index.html          # Main HTML file
├── style.css           # Stylesheet for the application
├── script.js           # JavaScript functionality
├── README.md           # Project documentation
└── assets/             # Images and other assets (if any)
    └── screenshot.png  # Application screenshot
```

## Technical Implementation

### Core Algorithm

The age calculation uses JavaScript's Date object to compute the difference between the birth date and the current date. The algorithm accounts for:

- Leap years and varying month lengths
- Negative day differences when the current day is less than the birth day
- Month borrowing for accurate day calculations
- Year adjustments when necessary

### Key Functions

- `calculateAge()`: Main function that computes age based on input values
- `validateDate()`: Ensures entered dates are valid and not in the future
- `updateDisplay()`: Updates the UI with calculated results
- `handleInputChange()`: Manages real-time input validation and calculation

## Browser Compatibility

This application is compatible with all modern browsers including:
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+
- Opera 47+

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Maintain the existing code style and structure
- Ensure all input validation remains intact
- Test thoroughly across different browsers
- Update documentation if adding new features
- Keep the application lightweight and dependency-free

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Inspired by the need for a simple, accurate age calculator
- Built with modern web standards and accessibility in mind
- Designed for educational purposes and practical use

## Contact

**Developer**: [chstridho]  
**GitHub**: [@chstridho](https://github.com/chstridho)

## Changelog

### v1.0.0 (Current)
- Initial release with core age calculation functionality
- Responsive design implementation
- Input validation and error handling
- Cross-browser compatibility

---

*For questions, suggestions, or bug reports, please open an issue in the [GitHub repository](https://github.com/chstridho/age-calculator/issues).*
