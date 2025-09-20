# Life-Line Air Drone Demo 🚁

An autonomous medical delivery platform simulation featuring real-time fleet monitoring, medical supply tracking, and mission analytics for VTOL (Vertical Take-Off and Landing) drones.

![Drone Demo](https://img.shields.io/badge/Status-Demo%20Ready-green)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow)
![HTML5](https://img.shields.io/badge/HTML5-Standard-orange)
![CSS3](https://img.shields.io/badge/CSS3-Modern-blue)

## 🌟 Overview

Life-Line Air Demo is an interactive web-based simulation platform that demonstrates autonomous medical delivery capabilities using VTOL drones. The system provides comprehensive mission planning, real-time telemetry monitoring, and medical payload management for emergency healthcare scenarios.

## ✨ Key Features

### 🎯 Mission Control
- **Interactive Dashboard** - Real-time system status and mission overview
- **Mission Planning** - Environment selection and payload configuration
- **Live Mission Control** - Start, pause, resume, and abort mission capabilities
- **Waypoint Navigation** - GPS-based flight path planning and execution

### 📊 Real-Time Monitoring
- **Telemetry Dashboard** - Live altitude, battery, speed, and temperature charts
- **System Status** - Component health monitoring (PX4 SITL, Gazebo, MAVLink)
- **Mission Timeline** - Visual progress tracking with waypoint status
- **Event Logging** - Comprehensive mission log with export functionality

### 🏥 Medical Payload Management
- **Emergency AED Kit** (3.2 kg) - Automated External Defibrillator with CPR supplies
- **Blood Transport Kit** (2.8 kg) - Temperature-controlled blood bag transport
- **Medication Delivery** (1.5 kg) - Emergency medications and epinephrine auto-injectors
- **Temperature Control** - Real-time payload temperature monitoring

### 🌍 Environment Scenarios
- **Forest Canopy** - GPS-denied navigation with dense vegetation challenges
- **Desert Plain** - Extreme weather simulation with dust/sand effects
- **Urban Environment** - Complex building obstacles and precision landing

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No additional software installation required

### Installation
1. **Clone the repository**
   ```bash
   git clone https://github.com/shashankchaurasiya27-boop/Life-Line-Air-Demo.git
   cd Life-Line-Air-Demo
   ```

2. **Open the application**
   - Simply open `index.html` in your web browser
   - Or serve it using a local web server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8000
   ```

3. **Access the demo**
   - Navigate to `http://localhost:8000` (if using a server)
   - Or double-click `index.html` to open directly

## 🎮 How to Use

### 1. Dashboard Overview
- View system status and mission readiness
- Monitor battery level, payload temperature, and signal strength
- Check flight time and system health indicators

### 2. Environment Selection
- Choose from Forest, Desert, or Urban scenarios
- Review environment-specific challenges and conditions
- Select appropriate mission parameters

### 3. Payload Configuration
- Select medical payload type (AED, Blood Transport, Medication)
- Review payload specifications and contents
- Configure temperature control settings

### 4. Mission Execution
- Click **START MISSION** to begin autonomous flight
- Monitor real-time telemetry and mission progress
- Use **PAUSE** to temporarily halt mission
- **EMERGENCY ABORT** for immediate mission termination

### 5. Telemetry Monitoring
- Switch to Telemetry Dashboard for detailed charts
- Monitor altitude profile, battery consumption, ground speed
- Track payload temperature and system performance

### 6. Mission Planning
- Configure cruise altitude (50-200m)
- Set cruise speed (5-25 m/s)
- Choose delivery method (Precision Landing, Air Drop, Winch Delivery)

## 📁 Project Structure

```
Life-Line-Air-Demo/
├── index.html          # Main HTML interface
├── app.js             # JavaScript application logic
├── style.css          # CSS styling and responsive design
└── README.md          # Project documentation
```

## 🔧 Technical Details

### Architecture
- **Frontend**: Pure HTML5, CSS3, and JavaScript (ES6+)
- **Charts**: Chart.js for real-time data visualization
- **Design System**: Custom CSS with CSS variables for theming
- **Responsive**: Mobile-first design with adaptive layouts

### Key Components
- **DroneDemo Class** - Main application controller
- **Telemetry System** - Real-time data simulation and updates
- **Mission Engine** - Waypoint navigation and progress tracking
- **UI Components** - Interactive dashboard and control panels

### Data Flow
1. **Environment Selection** → Mission parameters configuration
2. **Payload Selection** → Temperature control and weight calculations
3. **Mission Start** → Waypoint navigation and telemetry updates
4. **Real-time Monitoring** → Chart updates and status tracking
5. **Mission Completion** → Logging and data export

## 🎨 Design Features

### Visual Design
- **Modern UI** - Clean, professional interface design
- **Dark/Light Mode** - Automatic theme switching based on system preference
- **Color-coded Status** - Intuitive status indicators (Success, Warning, Error, Info)
- **Responsive Layout** - Optimized for desktop, tablet, and mobile devices

### User Experience
- **Intuitive Navigation** - Bottom navigation bar with clear icons
- **Real-time Feedback** - Immediate visual feedback for all actions
- **Accessibility** - Keyboard navigation and screen reader support
- **Performance** - Smooth animations and efficient data updates

## 📊 Mission Scenarios

### Forest Canopy Scenario
- **Challenges**: GPS signal degradation, dense canopy navigation, limited landing zones
- **Mission Type**: Search and rescue medical supply delivery
- **Weather**: Overcast, 15°C, Light wind
- **Waypoints**: 5-point navigation with altitude variations

### Desert Plain Scenario
- **Challenges**: Extreme temperature, dust interference, long range flight
- **Mission Type**: Emergency medical transport
- **Weather**: Clear, 35°C, Moderate wind with dust
- **Waypoints**: High-altitude cruise with extended range

### Urban Scenario
- **Challenges**: Building obstacles, air traffic, precision landing
- **Mission Type**: Hospital-to-hospital transport
- **Weather**: Partly cloudy, 22°C, Variable wind
- **Waypoints**: Building clearance and precision approach

## 🔍 API Reference

### DroneDemo Class Methods

#### Mission Control
- `startMission()` - Initialize and begin autonomous flight
- `togglePauseMission()` - Pause/resume mission execution
- `abortMission()` - Emergency mission termination
- `resetDemo()` - Reset all systems to initial state

#### Telemetry
- `updateTelemetryData()` - Simulate realistic telemetry updates
- `updateTelemetryDisplay()` - Update UI with current telemetry values
- `updateCharts()` - Refresh real-time data visualizations

#### Navigation
- `switchView(viewId)` - Navigate between application views
- `updateWaypoints()` - Update waypoint markers on map
- `centerMapView()` - Center map on drone position

#### Logging
- `addLogEntry(level, message)` - Add entry to mission log
- `exportLog()` - Export mission log as text file
- `clearLog()` - Clear mission event log

## 🚀 Future Enhancements

### Planned Features
- **Multi-drone Support** - Fleet management and coordination
- **Weather Integration** - Real-time weather data integration
- **3D Visualization** - Three-dimensional flight path visualization
- **Mobile App** - Native mobile application development
- **API Integration** - Real drone hardware integration capabilities

### Technical Improvements
- **WebSocket Support** - Real-time bidirectional communication
- **Database Integration** - Mission history and analytics storage
- **User Authentication** - Multi-user support and role management
- **Performance Optimization** - Enhanced rendering and data processing

## 🤝 Contributing

We welcome contributions to improve the Life-Line Air Demo platform!

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Follow existing code style and conventions
- Add comments for complex functionality
- Test changes across different browsers
- Update documentation for new features

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- **Shashank Chaurasia** - *Initial work* - [shashankchaurasiya27-boop](https://github.com/shashankchaurasiya27-boop)

## 🙏 Acknowledgments

- Chart.js for excellent data visualization capabilities
- Modern CSS techniques for responsive design
- VTOL drone technology inspiration from aerospace industry
- Medical emergency response protocols and best practices

## 📞 Support

For support, questions, or feature requests:
- Create an issue on GitHub
- Contact: [shashankchaurasiya27-boop](https://github.com/shashankchaurasiya27-boop)

---

**Life-Line Air Demo** - Advancing autonomous medical delivery through innovative drone technology 🚁⚕️
