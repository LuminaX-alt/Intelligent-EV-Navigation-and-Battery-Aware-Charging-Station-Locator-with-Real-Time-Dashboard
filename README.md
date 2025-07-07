# Intelligent-EV-Navigation-and-Battery-Aware-Charging-Station-Locator-with-Real-Time-Dashboard

This project presents a comprehensive solution for electric vehicle (EV) users, integrating smart navigation, real-time vehicle monitoring, and intelligent battery management into a unified system. The core objective is to assist EV drivers in dynamically planning their routes based on current battery state-of-charge (SoC), predicting battery consumption for the selected journey, and automatically recommending nearby charging stations when the battery is expected to deplete beyond a critical threshold.

<img width="1316" alt="image" src="https://github.com/user-attachments/assets/03e14c82-00af-4361-9859-2e384548c2f3" />

![image](https://github.com/user-attachments/assets/b5e68b06-056b-4702-825e-fb97086acdb7)


<img width="1328" alt="image" src="https://github.com/user-attachments/assets/c309956d-97c7-4369-8326-e6b934cb13c7" />

The system is developed entirely within Google Colab and utilizes OpenStreetMap for route planning and real-world EV charging station data. The user specifies a start and end location, and the system calculates the optimal route, predicts the battery consumption based on distance, and evaluates whether the vehicle can reach the destination without recharging. If the estimated battery drain exceeds a predefined safety margin, the system searches for charging stations along the route and recommends the most optimal one based on proximity and location context. This decision is reflected on an interactive map using dynamic markers for origin, destination, charging stations, and the suggested stop.


<img width="740" alt="image" src="https://github.com/user-attachments/assets/65aa87d3-8e5c-4384-a9f4-5b04aa9195f2" />

<img width="716" alt="image" src="https://github.com/user-attachments/assets/4d757454-5cfe-4d3a-8cfc-e0201ef2b1a5" />

<img width="1295" alt="image" src="https://github.com/user-attachments/assets/9a550472-ce80-4565-b0aa-0cfd6a1a3d5a" />


To enhance the system's interactivity and usability, a real-time EV dashboard is included. This dashboard simulates key vehicular parameters such as speed, RPM, battery level, and remaining range using animated gauge charts and bullet indicators. Users can interact with these values via sliders, mimicking live vehicle behavior. The interface also includes a live-updating time-series graph that tracks speed and RPM over time, allowing users to visualize driving behavior trends.

All simulated values are logged in real-time to a structured dataset using Pandas. At the end of each session, the log data can be exported as a CSV file for performance review, diagnostics, or integration with analytics tools.

<img width="1329" alt="image" src="https://github.com/user-attachments/assets/431617c1-fd03-48a3-bffc-81386e58d17a" />


The project leverages open-source mapping and visualization tools including Plotly, IPyWidgets, and Folium, and avoids dependency on paid APIs like Google Maps. It serves as a modular and extensible prototype that can be scaled for real-time integration with GPS hardware, OBD-II systems, or vehicle telematics platforms.

In conclusion, this project provides a functional prototype of an EV route planner with battery-aware charging stop recommendations, supported by an interactive dashboard that simulates and monitors vehicle performance. It addresses the real-world challenge of range anxiety by ensuring drivers are always informed of their battery condition and the nearest available charging infrastructure, ultimately promoting safer and more efficient EV navigation.

