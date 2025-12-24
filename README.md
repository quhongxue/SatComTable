LEO Satellite Pass Prediction Tool (Web Application)
Tool Overview:
This is a web-based tool designed for predicting flyovers (passes) of Low Earth Orbit (LEO) satellites. It calculates crucial data for satellite communication, such as pass times and Doppler shift, based on user-provided satellite and ground station information. The tool is built using the satellite.jsJavaScript library for accurate orbital calculations.
Key Features:
User-Friendly Interface:​ Clearly divided into two main functional sections for easy operation.
Customizable Parameters:​ Allows setting of local time, timezone, elevation mask, and multiple ground station locations.
Data Export:​ Enables exporting of calculated pass data to CSV files for further analysis.
Doppler Shift Calculation:​ Essential for planning satellite communication links.
📡 Part 1: 7-Day Pass Prediction
This section generates a forecast of when a specific satellite will be visible above a specified minimum elevation for up to 7 days.
Input Fields:
TLE Line 1 & Line 2:​ Input the satellite's Two-Line Element set for accurate orbit prediction.
Local Time:​ Set the starting date and time for the prediction.
🕒 Reset to Current Time:​ A button to quickly set the time to the present moment.
Timezone (UTC+X):​ Select your local timezone offset from UTC.
Elevation Mask (°):​ Set the minimum elevation angle (0-90 degrees) for a valid pass. Satellites below this angle are not calculated.
Ground Station Latitude/Longitude Table:
Index (1-10):​ Manage up to 10 different ground station locations.
Longitude & Latitude:​ Enter the geographical coordinates for each ground station.
Action Buttons:
🚀 Calculate Passes:​ Initiates the prediction calculation based on the inputs above.
📥 Export to CSV:​ Downloads the resulting pass schedule (AOS, LOS, max elevation, etc.) as a CSV file.
📡 Part 2: Satellite Position & Doppler Shift Calculation
This section calculates the real-time position (latitude, longitude, altitude) of a satellite during a specific pass and the corresponding Doppler shift for communication frequencies.
Input Fields:
Pass Index:​ Specify which pass (from the list generated in Part 1) to analyze.
Ground Station Index:​ Select which ground station (from the table in Part 1) to use as the reference point.
Ground Station Longitude & Latitude:​ These fields are automatically populated based on the selected ground station index.
Transmit Frequency (MHz) & Receive Frequency (MHz):​ Enter the communication frequencies to calculate the Doppler shift effect.
Action Buttons:
🚀 Calculate Position & Doppler:​ Starts the calculation to track the satellite's path and compute the frequency shift for the given pass.
📥 Export to CSV:​ Downloads the detailed data (timestamp, position, Doppler shift, etc.) for the analyzed pass as a CSV file.
