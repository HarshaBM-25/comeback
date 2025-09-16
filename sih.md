🌱 IoT Smart Farming System – README
Overview

The IoT Smart Farming System is a complete smart agriculture solution designed to help farmers monitor, automate, and predict farm conditions. It integrates real-time sensors, automation, cloud connectivity, mobile access, and yield prediction to optimize water usage, save electricity, and improve crop management. The system can also be connected to regional agricultural offices for expert guidance and large-scale monitoring.

Features
1. Real-Time Monitoring

Temperature & Humidity (DHT11/DHT22)

Gas Levels (MQ135)

Soil Moisture

Water Level in hydroponic or irrigation systems

2. Automation

Automatic irrigation using relays + NodeMCU

Triggers irrigation based on soil moisture and water level readings

3. Mobile App for Farmers

Real-time monitoring of farm conditions on Android/iOS

Alerts and notifications about low water, dry soil, or high gas levels

Easy-to-use, farmer-friendly interface in local language

4. Regional Agricultural Office Software

Monitors multiple farms in real-time

Aggregates sensor data and predicts regional and farm-level yield

Provides advisories, alerts, and resource planning for farmers

Helps policymakers make data-driven decisions for irrigation, subsidies, and crop management

System Architecture
[Sensors (Soil, Water, Temp, Humidity, Gas)]
            ↓
[Arduino / NodeMCU] → Collects sensor data
            ↓
[Python Core] → Sends data to Cloud / MySQL
            ↓
[Mobile App for Farmers] → Real-time monitoring + alerts
            ↓
[Automation Box] → Controls irrigation pumps
            ↓
[Regional Office Software] (Optional)
            → Receives data from multiple farms
            → Provides yield predictions, alerts, advisories

Hardware Components

Sensor Box 1: DHT11/DHT22 (Temp & Humidity), MQ135 (Gas)

Sensor Box 2: Soil Moisture Sensor, Water Level Sensor

Automation Box: NodeMCU + Low-Level Trigger + Relay

Software Components

Arduino Source Code (Devices folder)

Python Core → Sends sensor data → Cloud Database

Mobile App → Farmer-friendly real-time monitoring

Regional Office Software → Dashboard + yield prediction

Database → Cloud MySQL or Firebase (data_store.sql)

Installation Guide

Clone or Download Repository

git clone https://github.com/Deshan555/IOT-Smart_Farming.git


Setup Database

Use MySQL or a cloud database (Firebase/Cloud SQL)

Import data_store.sql

Upload Arduino Codes

Upload codes from Devices folder to respective NodeMCU / Arduino

Run Python Core

Executes scripts to send sensor data → Cloud Database

Mobile App for Farmers

Connect app to the cloud database to receive real-time sensor data and alerts

Regional Office Software

Connect to cloud database to monitor multiple farms, predict yield, and send advisories

Benefits for Farmers

Save Water & Electricity → automated irrigation

Prevent Crop Loss → alerts for low soil moisture or high gas levels

Plan Market & Harvest → farm-level yield prediction

Remote Monitoring → via mobile app anywhere

Expert Guidance → through advisories from regional agricultural office

Benefits for Regional Agricultural Offices

Monitor multiple farms in real-time

Aggregate sensor data for regional planning

Predict farm and regional yield → better market and subsidy planning

Send advisories and alerts → personalized guidance to farmers

Resource allocation → water distribution, irrigation schedules, fertilizer use

Future Enhancements

Local language voice alerts for farmers

AI-based pest/disease detection module

Solar-powered sensor boxes for energy efficiency

Offline-first operation for areas with poor internet connectivity

Integration with government schemes for automatic subsidy recommendations

Technologies Used

Hardware: Arduino, NodeMCU, DHT11/DHT22, MQ135, Soil Moisture, Water Level Sensors, Relay

Software: Python, MySQL / Firebase, Mobile App (Android/iOS), Web dashboard for regional office

Communication: Wi-Fi, GSM/4G, MQTT/HTTP

Cloud (Optional): AWS, GCP, Firebase, or any MySQL-compatible cloud DB

Summary

“IoT Smart Farming System monitors farm conditions in real-time, automates irrigation, predicts farm-level and regional yield, and provides farmers with actionable alerts and expert guidance through a mobile app, while enabling regional agricultural offices to make data-driven decisions.” 🌾📊
