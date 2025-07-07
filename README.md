# Dynamic Pricing Engine for Urban Parking Lots

This project simulates a dynamic pricing engine for 14 urban parking spaces using real-time data streams and basic economic principles. It is built entirely from scratch using Python, Pandas, NumPy, and Pathway — with Bokeh for real-time visualization.

##  Objective
To optimize parking space utilization by adjusting prices in real-time based on:
- Occupancy levels
- Queue length
- Traffic congestion
- Special events
- Vehicle type
- Competitor pricing (optional, Model 3)

##  Models Implemented

### Model 1: Baseline Linear Model
- Price increases linearly with occupancy.
- Smooth transitions using per-step and global bounds.

### Model 2: Demand-Based Pricing Model
- Demand is calculated from multiple features.
- Price is scaled relative to normalized demand.
- Ensures price is bounded between 0.5× and 2× base price.

### Model 3 (Optional): Competitive Pricing
- Incorporates competitor prices and geographic proximity.
- Suggests rerouting when necessary.

## Tech Stack
- **Data Processing**: Pandas, NumPy
- **Streaming**: Pathway
- **Visualization**: Bokeh + Panel
- **Notebook Environment**: Google Colab

##  Features
- Real-time pricing updates across all 14 lots
- Dynamic line plots for price trends
- Pricing model interpretable and smooth
- Modular structure for easy experimentation

##  Files
- `notebook.ipynb`: Full implementation of all models
- `stream_input.csv`: Cleaned dataset for streaming
- `README.md`: Project overview

##  How to Run
1. Install dependencies:  
   `!pip install pathway bokeh panel`

2. Open `notebook.ipynb` in Google Colab

3. Run all cells to:
   - Simulate live streaming with Pathway
   - Apply pricing models
   - Visualize real-time price adjustments with Bokeh

---

