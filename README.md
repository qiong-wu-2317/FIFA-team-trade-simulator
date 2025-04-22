# Football Team Finance Monitor Documentation

## Project Summary

The Football Team Finance Monitor is an interactive data visualization and analytics tool designed for football club managers and analysts. It provides comprehensive financial insights into player valuations, wage structures, and transfer market activities, offering actionable intelligence for squad planning and budget management.

The dashboard integrates roster analysis, transfer simulation, and financial visualization using D3.js. It includes predictive analytics to assess the financial impact of potential player transfers and salary changes.

## Key Features

### Player Roster Analysis

- **Value & Wage Distribution**: Histograms showing how player values and wages are distributed across the squad
- **Top Player Identification**: Automatic sorting to highlight highest-value and highest-earning players
- **Interactive Tables**: Detailed player information with sortable columns

### Transfer Market Simulation
- **Sell/Buy Lists**: Simulate player transfers by adding players to sell and purchase lists
- **Financial Impact Analysis**: Real-time calculation of transfer profits/losses
- **Squad Value Projection**: Forecasts updated squad value after transfers

### Financial Visualization
- **Dual-Axis Bar Charts**: Compare player values and wages side-by-side
- **Interactive Tooltips**: Hover over elements to see detailed financial information
- **Threshold Alerts**: Visual indicators for wage/value anomalies


## Component Structure

| Component Name | Description |
|----------------|-------------|
|roster | Array containing current squad players
|sellList | Players marked for transfer out
|purchaseList | Players targeted for transfer in
|teamFinanceMonitor | Main dashboard component
|teamRosterHistogram | Visualizes value/wage distribution
|playerFinanceTable | Interactive table of player finances
|transferSimulator | Interface for managing transfers

## External Libraries Used

### Data Processing & Visualization
- **d3.js (v7.0+)**: 
  - CSV parsing and data transformation
  - Advanced data manipulation and calculations
  - Dynamic visualization rendering

### Interactive Controls
- **@observablehq/inputs**:
  - Transfer budget sliders
  - Player filter dropdowns
  - Interactive threshold controls
  - Multi-select tables for roster management

### Specialized Components
- **advancedSingleSelector**:
  - Custom player selection interface
  - Threshold-based visual alerts
  - Styled data tables with sorting capabilities
  - Integrated tooltips for financial metrics

- **teamFinanceMonitor**:
  - Real-time financial forecasting engine
  - Squad value projection models
  - Wage structure analysis
  - Transfer impact simulation (both historical and predictive)
  - Automated report generation


## Observable Notebook

### FIFA Team Trade Simulator
**Notebook**: [FIFA Team Trade Simulator](https://observablehq.com/d/35d872661d7268c4)  
**Features**:
- Real-time player valuation tracking
- Interactive trade proposal interface
- Squad chemistry impact forecasting
- Financial fair play compliance checks
- Three-way trade simulation

### FIFA 2022 Full Dataset Importer
**Notebook**: [FIFA 2022 Full Dataset Importer](https://observablehq.com/d/55ec80ca780b07ed)
**Features**:
- Complete player stats import (over 90 attributes)
- Dynamic data filtering
- dashboard UI generator

## Project Usage

- Import data from FIFA 2022
- Select dataset scale based on leagues
- Select managed team
- Add players to the sell list to simulate outgoing transfers
- Add players to the purchase list to simulate incoming transfers
- View real-time updates to:
    - Squad market value
    - Wage budget
    - Net transfer profit/loss
    - Projected financial position


## Usage of GenAI  
version: ChatGPT 4o

### Data Visualization Optimization
Use Case: Developing effective D3.js visualizations for financial data
Prompt: "How can I create a dual-axis histogram comparing football player values and wages using D3.js?"

### UI/UX Design
Use Case: Creating an intuitive transfer simulation interface
Prompt: "How to design an interactive football transfer simulator with clear financial feedback?"

### Observable Integration
Use Case: Implementing reactive components in Observable
Prompt: "What's the best way to structure reactive financial calculations in Observable notebooks?"

### Performance Optimization
Use Case: Handling large squad datasets efficiently
Prompt: "How can I optimize D3.js visualizations for large football squad datasets?"


## Resourse
[Video](https://drive.google.com/file/d/1VSk3Mgq6gCwcm_atFodJ1pz4DYBAXJz8/view?usp=sharing)  
[Bluesky](https://bsky.app/profile/qiongwu.bsky.social/post/3lngpsoad3s2i)  
[Instructions Doc](Documentation.pdf)  

## License

MIT License
