# G-BUZZ

A comprehensive web dashboard for IIT Guwahati students featuring academic calendar, real-time weather, and placement analytics. Built with modern web technologies for an engaging user experience.

## 🌟 Features

### 📅 Academic Calendar
- **Official IITG Events**: Winter/Monsoon semester schedules
- **Festivals & Fests**: Alcheringa, Techniche, Udgam, Spirit
- **Examination Dates**: Mid-sem and end-sem schedules  
- **Important Deadlines**: Registration, course adjustments
- **Color-coded Events**: Easy visual identification
- **Responsive Timeline**: Mobile-friendly event cards

### 🌤️ Live Weather Integration
- **Real-time Data**: Live weather for Guwahati via OpenWeatherMap API
- **Comprehensive Info**: Temperature, humidity, wind speed, pressure
- **Weather Icons**: Visual weather condition indicators
- **Auto-refresh**: Updates every 10 minutes
- **IST Timestamps**: Local time zone support

### 📊 Placement Analytics
- **Department-wise Data**: CSE, ECE, ME, CE, EEE, CHE
- **Multi-year Statistics**: 2021-2024 placement trends
- **Interactive Charts**: Doughnut charts with animations
- **Key Metrics**: Placement rate, average package, highest package
- **Company Information**: Top recruiting companies

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- OpenWeatherMap API key (free registration)
- Internet connection for weather data

### Installation

1. **Download the Code**
   ```bash
   # Clone or download the HTML file
   git clone https://github.com/your-username/iitg-dashboard.git
   # OR download app.html directly
   ```

2. **Setup API Key**
   - Register at [OpenWeatherMap](https://openweathermap.org/api)
   - Get your free API key
   - Replace in `app.html`:
   ```javascript
   const API_KEY = 'YOUR_API_KEY_HERE'; // Line ~325
   ```

3. **Run the Dashboard**
   - **Option A**: Double-click `app.html` to open in browser
   - **Option B**: Use local server:
   ```bash
   python -m http.server 8000
   # Open http://localhost:8000
   ```

## 📁 File Structure

```
iitg-dashboard/
├── app.html                 # Main dashboard file
├── README.md               # This file
└── assets/                 # Optional assets folder
    ├── screenshots/        # Dashboard screenshots
    └── icons/             # Custom icons (if any)
```

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Custom CSS with gradients and animations
- **Charts**: Chart.js for data visualization
- **API**: OpenWeatherMap for weather data
- **Responsive**: Mobile-first design approach

## 📱 Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| Chrome  | 70+     | ✅ Full Support |
| Firefox | 65+     | ✅ Full Support |
| Safari  | 12+     | ✅ Full Support |
| Edge    | 79+     | ✅ Full Support |

## 🎨 Customization

### Modify Academic Events
Edit the `academicEvents` array in the JavaScript section:
```javascript
const academicEvents = [
    { 
        date: '2025-01-02', 
        title: 'Your Event', 
        type: 'academic', 
        description: 'Event description' 
    },
    // Add more events...
];
```

### Update Placement Data
Modify the `placementData` object:
```javascript
const placementData = {
    'CSE': {
        2024: { 
            placed: 85, 
            total: 95, 
            avg: 18.5, 
            highest: 55 
        }
    }
    // Update with real data...
};
```

### Change Color Scheme
Update CSS variables in the style section:
```css
:root {
    --primary-gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    --secondary-color: #1e3c72;
    --accent-color: #2a5298;
}
```

## 📊 API Usage

### Weather API
- **Provider**: OpenWeatherMap
- **Endpoint**: Current Weather Data
- **Rate Limit**: 1000 calls/day (free tier)
- **Update Frequency**: Every 10 minutes

### API Key Security
⚠️ **Important**: For production deployment, use environment variables:
```javascript
// For local development only
const API_KEY = process.env.WEATHER_API_KEY || 'fallback-key';
```

## 🌐 Deployment Options

### Free Hosting Platforms
1. **Netlify**
   - Drag and drop `app.html`
   - Auto-deploy from Git

2. **Vercel**
   - Import from GitHub
   - Instant deployment

3. **GitHub Pages**
   - Create repository
   - Enable Pages in settings

4. **Firebase Hosting**
   - `firebase init hosting`
   - `firebase deploy`

## 📈 Performance Features

- **Lazy Loading**: Images load on demand
- **Caching**: Weather data cached locally
- **Service Worker**: Offline support (optional)
- **PWA Ready**: Installable on mobile devices
- **Optimized Animations**: 60fps smooth transitions

## 🔧 Troubleshooting

### Weather Not Loading
1. Check API key is correctly placed
2. Verify internet connection
3. Check browser console for errors
4. Ensure API key is active (not expired)

### Charts Not Displaying
1. Ensure Chart.js loads properly
2. Check browser developer tools
3. Verify placement data format

### Mobile Issues
1. Test on different devices
2. Check viewport meta tag
3. Verify responsive CSS

## 🤝 Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

### Development Setup
```bash
# Clone repository
git clone https://github.com/your-username/iitg-dashboard.git

# Navigate to directory
cd iitg-dashboard

# Start local server
python -m http.server 8000

# Open browser
open http://localhost:8000
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **IIT Guwahati** for academic calendar data
- **OpenWeatherMap** for weather API
- **Chart.js** for visualization library
- **Community** for feedback and suggestions

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/your-username/iitg-dashboard/issues)
- **Email**: your.email@example.com
- **Documentation**: [Wiki](https://github.com/your-username/iitg-dashboard/wiki)

## 🗺️ Roadmap

### Version 1.1.0
- [ ] Dark mode implementation
- [ ] Export calendar to Google Calendar
- [ ] Email notifications for deadlines
- [ ] Multi-language support

### Version 1.2.0
- [ ] Student login integration
- [ ] Personal schedule management
- [ ] Grade tracking
- [ ] Assignment reminders

### Version 2.0.0
- [ ] Backend API integration
- [ ] Real-time notifications
- [ ] Mobile app version
- [ ] Advanced analytics

## 📸 Screenshots

### Desktop View
![Desktop Dashboard](assets/screenshots/desktop-view.png)

### Mobile View
![Mobile Dashboard](assets/screenshots/mobile-view.png)

### Placement Analytics
![Placement Charts](assets/screenshots/placement-analytics.png)

---

**Made with ❤️ for IIT Guwahati Students**

*Last updated: June 2025*
