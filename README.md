# Traffic Flow Analysis Dashboard

An interactive web-based application for analyzing highway traffic flow characteristics using classical traffic engineering models.



## 🚗 Overview

This dashboard implements three fundamental traffic flow models to analyze speed-flow-density relationships on highways and freeways. It provides real-time capacity calculations, Level of Service classifications, and interactive visualizations for transportation planning and operations.

## ✨ Features

- **Three Traffic Flow Models**
  - Greenshields Model (1935) - Linear speed-density relationship
  - Greenberg Model (1959) - Logarithmic relationship for congested conditions
  - Underwood Model (1961) - Exponential relationship for free-flow conditions

- **Real-Time Analysis**
  - Highway capacity calculation (vehicles per hour)
  - Critical density determination (vehicles per mile)
  - Critical speed identification (miles per hour)
  - Volume-to-capacity ratio computation

- **Interactive Visualizations**
  - Speed-Density relationship curves
  - Flow-Density relationship curves
  - Speed-Flow scatter plots
  - Dynamic parameter adjustments

- **Level of Service (LOS) Assessment**
  - Automated LOS classification (A through F)
  - Based on Highway Capacity Manual methodology
  - Multiple traffic volume scenarios


## 🛠️ Technologies Used

- **React 18.2.0** - Frontend framework
- **Recharts 2.10.3** - Data visualization library
- **Tailwind CSS** - Styling and responsive design
- **JavaScript (ES6+)** - Core programming language
- **HTML5** - Markup structure

## 📊 Traffic Flow Models

### Greenshields Model
The most widely used model with linear speed-density relationship:
```
Speed: u = uf × (1 - k/kj)
Flow: q = k × uf × (1 - k/kj)
```

### Greenberg Model
Logarithmic model suited for congested conditions:
```
Speed: u = uf × ln(kj/k)
Flow: q = k × uf × ln(kj/k)
```

### Underwood Model
Exponential model optimal for free-flow:
```
Speed: u = uf × exp(-k/ko)
Flow: q = k × uf × exp(-k/ko)
```

Where:
- `uf` = Free-flow speed (mph)
- `kj` = Jam density (veh/mi)
- `k` = Current density (veh/mi)

## 🚀 Getting Started

### Option 1: View Online (Easiest)
Simply visit the 

### Option 2: Run Locally
1. Download `index.html` from this repository
2. Open the file in any modern web browser
3. No installation or setup required!



## 📖 How to Use

1. **Adjust Input Parameters**
   - Free-Flow Speed: Set highway design speed (45-75 mph)
   - Jam Density: Set maximum vehicle density (100-250 veh/mi)
   - Model Selection: Choose between Greenshields, Greenberg, or Underwood

2. **Analyze Results**
   - View calculated road capacity in the metrics cards
   - Examine speed-flow-density relationship charts
   - Review Level of Service classifications for sample flows

3. **Interpret Findings**
   - Compare different model behaviors
   - Understand capacity and critical operating points
   - Assess LOS for various traffic volumes

## 🎓 Use Cases

- Highway Capacity Planning - Determine required lanes for design volumes
- Traffic Operations - Predict congestion and implement management strategies
- Impact Studies - Assess development effects on roadway capacity
- Education - Visualize traffic flow theory concepts
- **Research** - Compare theoretical models with field data

## 📚 Background

This project demonstrates the application of fundamental traffic flow theory in a modern, interactive format. Traffic flow models help transportation engineers:

- Design highways with adequate capacity
- Predict when and where congestion will occur
- Evaluate impacts of new developments
- Optimize traffic signal timing
- Implement effective traffic management strategies

The three models implemented represent different eras and approaches in traffic flow theory, each with unique strengths for different traffic conditions.

## 🔧 Technical Details

### Architecture
- Single-page application (SPA) design
- Component-based React architecture
- Memoized calculations for performance optimization
- Responsive design for mobile and desktop

### Performance
- Real-time calculations (< 50ms response time)
- 100 data points per model for smooth curves
- Efficient re-rendering with React hooks
- Optimized for modern browsers

### Browser Compatibility
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 📈 Future Enhancements

- [ ] Data import/export functionality (CSV)
- [ ] Model calibration with field data
- [ ] Multi-lane capacity analysis
- [ ] Time-series traffic pattern analysis
- [ ] Weather and incident impact modeling
- [ ] Shock wave and queue analysis
- [ ] Report generation (PDF export)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author
**Ashish Basnet**  
- Graduate Student, Transportation Engineering
- University of New Mexico
- Email: asinghbasnet@unm.edu


## 🙏 Acknowledgments

- Based on classical traffic flow theory by Greenshields (1935), Greenberg (1959), and Underwood (1961)
- Highway Capacity Manual (HCM) for Level of Service methodology
- Transportation engineering coursework at UNM

