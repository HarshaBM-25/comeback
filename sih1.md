                 ┌─────────────────────┐
                 │    SENSOR BOXES     │
                 │--------------------│
                 │- Temp & Humidity   │
                 │- Gas (MQ135)       │
                 │- Soil Moisture     │
                 │- Water Level       │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌─────────────────────┐
                 │   NODEMCU / ARDUINO │
                 │--------------------│
                 │ Collects sensor     │
                 │ readings            │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌─────────────────────┐
                 │   PYTHON CORE       │
                 │--------------------│
                 │ Sends data to       │
                 │ Cloud / MySQL DB    │
                 └─────────┬──────────┘
                           │
            ┌──────────────┴──────────────┐
            │                             │
            ▼                             ▼
 ┌─────────────────────┐         ┌────────────────────────┐
 │  MOBILE APP FOR      │         │ REGIONAL OFFICE        │
 │      FARMERS         │         │ DASHBOARD + YIELD      │
 │--------------------- │         │ PREDICTION SOFTWARE    │
 │- Real-time monitoring│         │------------------------│
 │- Alerts & notifications │       │- Monitor multiple farms│
 │- Local language support │       │- Predict regional yield│
 └─────────┬───────────┘         │- Send advisories/alerts│
           │                     └───────────┬────────────┘
           │                                 │
           ▼                                 ▼
 ┌─────────────────────┐           ┌─────────────────────┐
 │ AUTOMATION BOX      │           │ POLICY & RESOURCE   │
 │---------------------│           │ MANAGEMENT          │
 │- Controls irrigation │           │- Water allocation   │
 │  pumps automatically │          │- Irrigation schedules│
 │- Saves water & energy │          │- Fertilizer guidelines│
 └─────────────────────┘           └─────────────────────┘
