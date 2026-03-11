# Air-Quality-Simulation
Project for the course Modelització i Simulació de Sistemes in the Bachelor’s Degree in Artificial Intelligence (FIB, UPC). System Dynamics model that analyzes the impact of urban population and vehicle fleets on CO2 emissions and air quality using Insight Maker. 

This project focuses on the environmental impact of urban mobility. It models how demographic changes and the transition to cleaner vehicles affect the total accumulation of greenhouse gases.
The system is defined by four main stocks:
- Població (Population): Managed by birth, mortality, and migratory flows (immigration/emigration).
- Vehicles en Ús (Vehicles in Use): Driven by new vehicle purchases and the retirement of old ones.
- Qualitat Aire (Air Quality): An accumulator of total CO_2 emissions.
- Programes (Programs): A stock representing the implementation of environmental policies.

The system allows:
- Demographic Analysis: Simulating population growth based on real-world rates (1,701,891 initial inhabitants).
- Emission Forecasting: Calculating monthly CO_2 based on vehicle count and average emission factors (0.175 tons/vehicle).
- Scenario Comparison: Testing the efficiency of "Improvement Scenarios" (Millora) by adjusting technological impact factors.
- Long-term Projection: Evaluating environmental health over periods ranging from 600 to 1200 months.

The implementation follows a System Dynamics approach using the RK4 (Runge-Kutta 4th Order) numerical integration method. 
The project is divided into three iterative models:
- MODEL_BASE: The baseline scenario representing current trends without intervention.
- MILLORA1: An intervention scenario focusing on technological efficiency, reducing vehicle emission impact to 60%.
- MILLORA2: A structural change scenario starting with a 50% reduction in the initial vehicle fleet and a lower purchase rate (70%) over a double time horizon.

How to RunGo to Insight Maker.
  Click on "Make a Model" and select "Upload".
  Choose one of the provided files:
    MODEL_BASE.InsightMaker
    MILLORA1.InsightMaker
    MILLORA2.InsightMaker
  Once loaded, click the "Simulate" button to view the time-series graphs for population, vehicles, and CO2 levels.
