# Solar-Storage-Microgrid-Sim

## Project Overview

This project, **Solar-Storage-Microgrid-Sim**, aims to create a simple yet comprehensive simulation environment for a photovoltaic (PV) panel, battery, and inverter system integrated with the electrical grid. The simulation also interfaces with real-time energy pricing from the Electric Reliability Council of Texas (ERCOT) to enable dynamic economic decision-making based on current market conditions. (Note I was going to use the gridstatus ERCOT API but instead I may loop through existing days data to simulate real time data to make it easier for anyone to use without an API key.)

## Key Components

1. **PV Panel Simulation**: Models the behavior of solar panels over time, accounting for variables such as sunlight intensity and angle to predict energy production throughout the day.
2. **Battery Storage Model**: Simulates a battery system with realistic charge and discharge cycles, including efficiency losses and capacity limits that change as the battery charges or discharges.
### (Future)
3. **Inverter System**: Converts the DC output from the solar panels and battery storage into AC, mimicking the function of a real-world inverter with sinusoidal output waveform generation.
4. **Economic Analysis**: Integrates ERCOT energy pricing to calculate potential revenue from energy fed back into the grid, supporting strategic operational decisions for maximum economic benefit.

## Objective

The primary goal is to provide a tool for analyzing and optimizing the performance and economic returns of solar storage systems. This simulator will help in understanding how various factors, such as energy price fluctuations and storage capacity, impact the overall efficiency and profitability of solar power systems.

## Technology Stack

- **Python**: Utilized for its libraries listed below specific to modeling pv system and batteries, the ease of data integration with pandas for ERCOT data, and acess to visualization libraries and potentially ML libraries down the line.
- **Jupyter Notebook**: Used to allow me to prototype segments of code and comment on the process better
- **Libraries**: Uses `pvlib` for PV system simulation, `PyBaMM` for battery management, and other Python packages for data handling and visualization.
