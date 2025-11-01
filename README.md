# Weather Now 🌤️

A beautiful, responsive weather application built with vanilla HTML, CSS, and JavaScript. Get real-time weather information for any location worldwide with an intuitive interface and delightful animations.

![Design preview](./preview.jpg)

## ✨ Features

### Core Features
- 🔍 **Location Search** - Search for weather information by city, country, or coordinates
- 🌡️ **Current Weather** - Real-time temperature, conditions, and weather icons
- 📊 **Weather Metrics** - "Feels like" temperature, humidity, wind speed, and precipitation
- 📅 **7-Day Forecast** - Daily weather predictions with high/low temperatures
- ⏰ **Hourly Forecast** - Detailed 24-hour forecast with day selector
- 🌍 **Geolocation** - Automatic weather detection based on your current location
- ⭐ **Favorites** - Save and quickly access your frequently checked locations
- 🌓 **Theme Toggle** - Switch between light and dark themes
- 🎛️ **Unit System** - Toggle between Metric/Imperial units with granular controls

### Enhanced Features
- 🎨 **Dynamic Animations** - Weather-based particle effects and background animations
- ♿ **Accessibility** - Full keyboard navigation, screen reader support, and ARIA labels
- 📱 **Responsive Design** - Optimized for mobile, tablet, and desktop devices
- 💾 **Local Storage** - Saves your preferences and favorite locations
- ⚡ **Performance Optimized** - Debounced search, efficient DOM updates, and optimized animations

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, or Edge)
- Internet connection for API calls

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Umarcss/Weather-App.git
   cd Weather-App-main
   ```

2. **Open the application**
   - Simply open `index.html` in your web browser
   - Or use a local development server:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js
     npx serve
     ```

3. **Access the app**
   - Navigate to `http://localhost:8000` (if using a server)
   - Or directly open `index.html` in your browser

## 🎯 Usage

1. **Search for a location**
   - Type a city name, country, or location in the search bar
   - Select a result from the dropdown
   - Click "Search" or press Enter

2. **Add to favorites**
   - Click the checkmark icon next to the location name
   - Access saved locations via the "Favorites" dropdown in the header

3. **Change units**
   - Click the "Units" button in the header
   - Customize temperature, wind speed, and precipitation units

4. **Toggle theme**
   - Click the sun/moon icon in the header to switch themes

5. **View forecasts**
   - Scroll down to see the 7-day daily forecast
   - Check the hourly forecast for detailed temperature changes
   - Select different days from the dropdown to view hourly data

## 🛠️ Technology Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom properties, Grid, Flexbox, animations
- **Vanilla JavaScript (ES6+)** - No frameworks or dependencies
- **Open-Meteo API** - Free weather and geocoding services

## 📁 Project Structure

```
Weather-App-main/
├── index.html              # Main HTML file
├── styles.css              # Complete CSS with design system
├── script.js               # JavaScript functionality
├── style-guide.md          # Design specifications
├── README.md               # Project documentation
├── assets/
│   ├── images/             # Weather icons and UI assets
│   └── fonts/              # Custom fonts (DM Sans, Bricolage Grotesque)
└── design/                 # Design mockups and reference images
```

## 🎨 Design System

### Colors
- **Neutral Palette**: 9 shades from dark (`hsl(243, 96%, 9%)`) to white
- **Accent Colors**: 
  - Blue: `hsl(233, 67%, 56%)`
  - Orange: `hsl(28, 100%, 52%)`

### Typography
- **Primary Font**: DM Sans (Light, Medium, SemiBold, Bold, SemiBold Italic)
- **Display Font**: Bricolage Grotesque (Bold)
- **Base Size**: 18px

### Responsive Breakpoints
- **Mobile**: 375px (design) / 320px - 768px (actual)
- **Tablet**: 768px - 1024px
- **Desktop**: 1440px (design) / 1024px+ (actual)

## 🌐 API Information

This application uses the [Open-Meteo API](https://open-meteo.com/), a free weather API that requires no API key:

- **Weather API**: `https://api.open-meteo.com/v1/forecast`
- **Geocoding API**: `https://geocoding-api.open-meteo.com/v1/search`

Both APIs are free to use and don't require authentication.

## ♿ Accessibility

- ✅ Full keyboard navigation support
- ✅ Screen reader compatible with ARIA labels
- ✅ Semantic HTML structure
- ✅ Focus indicators for all interactive elements
- ✅ Reduced motion support (respects user preferences)
- ✅ High contrast mode compatible

## 🔧 Customization

### Adding Weather Icons
1. Add new icon files to `assets/images/`
2. Update the `WEATHER_CODES` object in `script.js`
3. Map weather codes to your new icons

### Modifying Themes
1. Update CSS custom properties in the `:root` and `[data-theme]` selectors in `styles.css`
2. Customize colors, backgrounds, and particle effects

### Extending API Data
1. Modify API parameters in the `getWeatherData()` function
2. Update display functions to show new data
3. Add corresponding HTML elements and CSS styles

## 🚀 Performance Features

- Debounced search input to reduce API calls
- Efficient DOM updates with minimal reflows
- Optimized animations using `requestAnimationFrame`
- Lazy loading for weather particles
- Local storage for caching preferences

## 🐛 Troubleshooting

### Common Issues

**Location not found?**
- Try different search terms or check spelling
- Use city name followed by country (e.g., "Paris, France")

**Weather data not loading?**
- Check your internet connection
- Open browser console for error messages
- Ensure the API endpoints are accessible

**Geolocation not working?**
- Ensure HTTPS is enabled (required in production)
- Grant location permissions when prompted
- Check browser settings for location access

**Performance issues?**
- Disable animations in browser accessibility settings
- Check browser console for any JavaScript errors

## 📱 Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 🎓 Learning Resources

This project demonstrates:
- Vanilla JavaScript ES6+ features
- CSS Grid and Flexbox layouts
- CSS Custom Properties (CSS Variables)
- API integration and data fetching
- Local storage management
- Responsive design principles
- Accessibility best practices
- Performance optimization techniques
