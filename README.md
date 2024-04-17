# G26_SC407

Mechanism 
Mechanism:
1.	Data Collection:
○	The system continuously monitors:
■	Home energy demand (real-time power usage)
■	Grid power availability (checks for outages)
■	EV battery state of charge (SOC)
■	Grid electricity prices (if participating in energy trading)
○	Historical data on usage patterns and outage frequency can be used for prediction.
2.	Decision Making:
○	An optimization algorithm analyzes the collected data and makes decisions based on pre-defined priorities:
■	Priority 1: Maintain Critical Loads: Ensure enough EV battery reserve to power critical home appliances (fridge, medical equipment) during outages.
■	Priority 2: Minimize Cost: If the grid is operational, prioritize charging the EV during off-peak hours for lower electricity costs.
3.	Control Actions:
○	Based on the decision, the algorithm triggers actions:
■	Grid Outage:
■	If a grid outage occurs and home demand exceeds critical load, the system automatically switches to discharge power from the EV battery to meet remaining home energy needs.
■	Grid Available:
■	If the grid is operational:
■	During off-peak hours, the system prioritizes charging the EV battery.
■	During peak hours, the system might limit charging or even discharge power back to the grid (V2G) if profitable and battery SOC allows
